# ph-rv-metabolomics

Analysis notebooks and environment metadata for a pulmonary hypertension right ventricular metabolomics project. The repository is intended to support manuscript review and reproducibility without distributing raw participant-level data.

## Graphical Abstract

The graphical abstract is included at `assets/graphical_abstract.png`.

![Graphical abstract](assets/graphical_abstract.png)

## Repository Structure

- `notebooks/`: R/Jupyter notebooks for univariate regression, pathway analysis, interaction analyses, MET-RV scores, REVEAL scores, and normality checks.
- `config/`: Non-sensitive analysis configuration.
- `renv.lock`: R package lockfile used to reproduce the package environment.
- `renv/`: `renv` bootstrap files. The local package library is intentionally ignored.
- `data/`: Placeholder only. Raw and processed data files are not included.
- `outputs/`: Placeholder only. Generated spreadsheets and other analysis outputs are not included.
- `metrv_models/`: Placeholder only. Generated model coefficient files are not included.
- `assets/`: Public repository assets, including the graphical abstract.

## Restore the R Environment

Install R and the `renv` package, then restore the package library from the lockfile:

```r
install.packages("renv")
renv::restore()
```

The project `.Rprofile` activates `renv` automatically when the repository is opened in R.

## Data Availability

Raw data, participant-level clinical files, metabolomics objects, and derived analysis outputs are not committed to this repository. To rerun the notebooks, place approved local copies of the required data files under `data/` using the paths referenced by the notebooks and project configuration.
