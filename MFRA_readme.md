## MFRA - Motif and Flanking Region Accessibility
MFRA is a Python-based analysis pipeline for quantifying motif accessibility and its flanking region accessibility in target and non-target RNAs using precomputed RNA secondary structure predictions.



## Dependencies and Reproducibility
MFRA was originally developed and run using Python 3.8.3 and standard scientific Python libraries (numpy, pandas, SciPy, Biopython, and matplotlib).
A minimal conda environment reproducing the original analysis environment is provided in `mfra_environment.yml` and can be created and activated as follows:



```
conda env create -f mfra_environment.yml
conda activate mfra
```
This environment is recommended if users encounter conflicts due to pre-existing package version differences. 

## External Dependencies
RNA secondary structure accessibility was computed using *RNAplfold* from the ViennaRNA package (v2.5.1). Later versions of ViennaRNA may produce output files with different formats. ViennaRNA must be installed separately [here](https://www.tbi.univie.ac.at/RNA/ViennaRNA/doc/html/install.html) and is not included in this repository.



## Input Requirements
(1) List of target transcripts (text file; one FBtr entry per line)
(2) List of non-target transcripts (text file; one FBtr entry per line)
(3) RNA motif (can be degenerate)
(4) Directory of *RNAplfold* outputs 

If you use MFRA, please cite the following:
[Manuscript in preparation]







