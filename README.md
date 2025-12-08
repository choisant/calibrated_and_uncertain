# Foundational modeling
This is a research project on uncertainty quantification for classification problems using various machine learning methods.

The project has resulted in the paper "Calibrated and Uncertain? Evaluating uncertainty estimates in binary classification models". The paper is still in the preprint stage and can be found on [ArXiv](https://arxiv.org/abs/2508.11460). The code used in the paper can be found in this repo, specifically in the `\src` and `experiments\gamma_n_dims` folders.

There is also a project in the `experiments\robot` folder which is the basis for a short lecture-series on infinite population inference logic.

## Apptainer container
This container is used to enable the usage of the R-packages used in this project. It includes a new version of Ubuntu as well as an installation of R and some packages needed to run the 'inferno' software. To use it, make sure Apptainer is installed, then build the container with the command

```
apptainer build env.sif apptainer.def 
```
To install the R-package, open the container and install the package in R, either directly from github or from a local copy.
