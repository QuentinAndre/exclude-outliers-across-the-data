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

## Citation

To cite this work, please cite the published article (see [`CITATION.cff`](CITATION.cff) for machine-readable metadata):

> André, Q. (2021). Outlier Exclusion Procedures Must be Blind to the Researcher's Hypothesis. *Journal of Experimental Psychology: General*. https://doi.org/10.1037/xge0001069

Paper page: https://quentinandre.net/publications/outliers-blind-hypothesis/

## License

- Original **code** by the author is released under the [MIT License](LICENSE).
- Original **text and figures** are released under [CC-BY-4.0](LICENSE-CC-BY-4.0.txt).
- The **Cao, Kong & Galinsky (2020)** data in `Data/` remains under its original license and terms.