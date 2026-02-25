# Calibrated and Uncertain? Evaluating uncertainty estimates in binary classification models
This is a research project on uncertainty quantification for classification problems using various machine learning methods.

The project has resulted in the paper "Calibrated and Uncertain? Evaluating uncertainty estimates in binary classification models" which was accepted for publication in the open access journal "Machine Learning: Science and Technology" 13 February 2026, with DOI:[10.1088/2632-2153/ae45ed](https://iopscience.iop.org/article/10.1088/2632-2153/ae45ed).

The paper with appendix describes the method used in the study thoroughly. All the code used to produce the results in the paper can be found in this repository.

## Data
The synthetic dataset used in the study can be found in the folder `experiments/gamma_n_dims/data`. The code used to generate data is contained in the jupyter notebook `experiments/gamma_n_dims/generate_data.ipynb`.

## Machine learning
The code for the different machine learning methods that are not contained within a python package can be found in the `src/` folder.

## Requirements
Python v3.10.4

Python packages
- scikit-learn v1.3.2
- scipy v1.11.4
- torch v2.6.0
- seaborn v0.13.2
- pandas v2.3.2
- numpy v1.26.3
- matplotlib v3.6.2

R v4.5.2
R packages
- [Inferno](https://github.com/pglpm/inferno) v0.2.1

## Apptainer container
This container is used to enable the usage of the R-packages used in this project. It includes a new version of Ubuntu as well as an installation of R and some packages needed to run the `inferno` software. To use it, make sure Apptainer is installed, then build the container with the command

```
apptainer build env.sif apptainer.def 
```
To install the R-package, open the container and install the package in R, either directly from github or from a local copy.
