# Agent & LLM Guide

This repository holds the data, materials, and analysis code for a published
research paper. If you are an AI agent or LLM working in this repo, start here.

## What this is

- **Paper:** Outlier Exclusion Procedures Must be Blind to the Researcher's Hypothesis
- **Author:** Quentin André
- **Published in:** Journal of Experimental Psychology: General (2021)
- **DOI:** https://doi.org/10.1037/xge0001069
- **Paper page:** https://quentinandre.net/publications/outliers-blind-hypothesis/
- **Citation:** see `CITATION.cff` — cite the **article**, not the repository.

## Layout

`README.md` is the authoritative description of the contents. In brief:
`Analysis.ipynb` and `Bayesian Analysis.ipynb` (with `.html` exports) contain the
code, figures, and results; `Data/` holds the reanalyzed data; `Buffer/` holds
pre-computed intermediate results; `Figures/` and `Literature Survey/` hold the
paper's figures and the JEP:General keyword survey.

## Reproducing the analysis

Python (Jupyter). Create the conda environment with
`conda env create --name outliers --file environment.yml`, activate it, and run
the notebooks. See `README.md` for details.

## Conventions & gotchas for agents

- **Office/PDF files:** `.docx` and `.pdf` are binary — do not read them
  directly. Convert first (e.g., `pandoc file.docx -t markdown`, or a
  PDF-to-markdown tool) and read the output.
- **Third-party data:** `Data/` contains the original data of Cao, Kong &
  Galinsky (2020), retrieved from https://osf.io/e8xnz/. It is not the authors'
  own data — see the License section before reusing.
- **Long-running code:** `Buffer/` exists because some computations (simulated
  experiments, simulated p-values, Bayesian traces) are expensive. Reuse the
  cached buffers rather than recomputing unless asked.

## License

- Original **code** by the author: MIT (see `LICENSE`).
- Original **text and figures**: CC-BY-4.0 (see `LICENSE-CC-BY-4.0.txt`).
- The **Cao, Kong & Galinsky (2020)** data in `Data/` remains under its original
  license and terms.
