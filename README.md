# Repository Structure

## .ipynb files
These files are Jupyter notebooks. They contain all the code necessary to reproduce the figures and results reported in the main manuscript.

To reproduce the analysis: 

1. Clone the repository
2. Run `conda env create --name outliers --file environment.yml` to create a conda environment with all the required data and libraries. You will need to install the [Anaconda Distribution][2] first if you do not have it.
3. Activate the environment using `conda activate outliers` and run the notebook.


## .html files
These files are exports of the Jupyter notebooks. They also contain all the figures, code, and results, but are not interactive.

## Literature Survey
This folder contains the survey of the JEP:General paper containing the keyword "outlier" published in 2019 and 2020.

## Figures
This subfolder contains the figures of the paper.

## Buffer
This subfolder contains pre-computed data that would be computationally expensive to recompute every time:

* The simulated experiments
* The simulated p-values in the data of Cao, Kong and Galinsky (2020)
* The Bayesian traces


## Data
This subfolder contains the original data of Cao, Kong and Galinsky (2020),
retrieved from [the OSF repository of the paper][1].


  [1]: https://osf.io/e8xnz/
  [2]: https://www.anaconda.com/distribution/