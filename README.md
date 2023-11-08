# An elevated rate of whole-genome duplication events in cancers from Black patients

This repository represents the computational analysis for the investigation of WGD racial disparities as conducted in the Sheltzer Lab.

## Data Availability

Some of the data used in this project are not publicly available. Below is a breakdown of the data that this project relies upon, specifically what it represent and whether it is publicly available.

+ `impact-505.csv`: Contains the HUGO symbols for the IMPACT-505 geneset, publicly available
+ `MSK-WGD.csv`: WGD data from the original cohort study, publicly available
+ `msk-met-cell2022-ancestry.tsv`: Ancestry determinations for MSK-MET patients following the method of Arora, et al. (2022), non-public data provided by Kanika Arora
+ `regionalLN.csv`: Metastasis data from Nguyen, et al. (2022), publicly available
+ cBioPortal data for MSK-MET: mutational, copy number, sample, and patient data that is publicly available from cBioPortal under project `msk_met_2021`
+ `pancan_pcawg_2020_clinical_data.csv`: Clinical data for PCAWG, publicly available
+ `TCGA_Demographics.csv` and `TCGA_arm_scores.csv`: Clinical and aneuploidy data for TCGA, publicly available

## Package Management

This project uses `renv` for package management. It should be sufficient to first install `renv` from within an R console:

```r
install.packages("renv")
```

Then to install all the necessary packages, from an R console in the root of this project:

```r
renv::restore()
```

This will install all the necessary packages and place then in a directory under `renv/library/` -- which will be loaded by default in most cases, but can be forced via `source("renv/activate.R")`.
