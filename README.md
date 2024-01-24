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

## System Requirements
### Software Dependencies

This project uses `renv` for dependency management. It should be sufficient to first install `renv` from within an R console:

```r
install.packages("renv")
```

Then to install all dependencies, from an R console in the root of this project:

```r
renv::restore()
```

This will install the specified versions of dependencies as listed in the `renv.lock` file, placing them in a directory under `renv/library/` -- which will often be loaded by default upon opening the RProject, but can be forced via `source("renv/activate.R")` from within an R console. The dependency installation process can take up to an hour if compiling all dependencies from source, but typically takes less than 30 minutes.

### Operating Systems

This project has been successfully run on Windows, Linux (Ubuntu family), and MacOS (Intel based) distributions. 

### Hardware

No non-standard hardware is required to run this project.

## Running the Project

If you have RStudio installed, you can double-click the `wgd_disparities.Rproj` file to open the project from your file manager. Once the project is open in RStudio, open the `wgd_disparities.Rmd` file. Just above where the file opens there will be a button labeled `Knit` -- clicking this button will run the code and produce an HTML report called `wgd_disparities.html`. Open this report in your preferred web browser to read the report. Running the project can take 20-40 minutes on a normal desktop computer.
