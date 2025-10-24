# Charlottesville Weather Forecast Project

This repository contains a dataset of historical weather data for Charlottesville, VA, as well as scripts and outputs to forecast 2024 monthly average temperatures. Our project analyzes trends, seasonality, and anomalies in monthly minimum and maximum temperatures from 2000–2023 using ARIMA modeling. The cleaned dataset, exploratory analyses, and model predictions are included to enable reproduction of all results.

## Contents of this repository
This repository contains everything needed to reproduce the analyses and results for this project: raw and cleaned weather data, R scripts for preprocessing and analysis, output plots, and predicted 2024 temperature data. The sections below outline software requirements, repository structure, and step-by-step instructions to reproduce the results.

---

## Section 1: Software and platform

**Software Used:**
- R Studio for data cleaning, exploratory analysis, and ARIMA modeling.
- Git for version control and GitHub for hosting.

**Add-on R packages required (install with `install.packages()` or via `renv`)**
- `tidyverse` (includes `dplyr`, `ggplot2`, `readr`, `tibble`, etc.)
- `rmarkdown`, `knitr` (rendering reports) , `vader`, `forecast`

## Section 2: Map of Documentation

 1. **DataFolder**
  - AverageTemps.csv – Full dataset with months and years, as well as the mean maximum and minimum temperature values used in analysis. 
  - Metadata.md – Metadata description file. 
  - mean_max_monthly_temps_2000_2025.csv – Just the mean maximum monthly temperature data. 
  - mean_min_monthly_temps_2000_2025.csv – Just the mean mimimum monthly temperature data. 
 2. **OUTPUT**
  - 1jantrends.png – Scatter plot with line of best fit of the mean minimum and maximum temperatures in January from 2000-2025. 
  - 2juntrends.png – Scatter plot with line of best fit of the mean minimum and maximum temperatures in June from 2000-2025. 
  - 3maxtimeseries.png – Decomposition of the additive time series of our maximum temperature data, which shows seasonal and nonseasonal trends.
  - 4mintimeseries.png – Decomposition of the additive time series of our minimum temperature data, which shows seasonal and nonseasonal trends. 
  - 6ModelPDF.pdf – Full project analysis for building time series model with minimum and maximum temperature data. <br>
 3. **SCRIPTSFolder**
  - Data Cleaning.Rmd – Data cleaning script where data is joined as well as general cleaning as well creation of EDA plots.
  - Model Building.Rmd – Model building script where time series model is fitted.


## Section 3 – How to Reproduce Our Results

If you want to reproduce our analysis and see all the figures and tables from our project, follow these steps:

1. **Get the Repository**
   - Clone the repo using Git:
     ```bash
     git clone https://github.com/hildj/DS-4002-Project1.git
     ```
   - Or download it as a ZIP file and extract it.
   - Open RStudio and set your working directory to the project folder.

2. **Make Sure the Data Files Are There**
   - The following CSV files need to be in the **same folder** as `AnalysisProject1.Rmd`:
     - `AmazonWithScores.csv`
     - `trainingdata.csv`
     - `testdata.csv`
   - These files are included in the repository, so you shouldn’t need to download anything else.

3. **Install R and Packages**
   - We used **R** (version 4.0 or higher) and RStudio.
   - Install the packages we used if you don’t already have them:
     ```r
     install.packages(c("tidyverse", "dplyr", "ggplot2",
                        "tidytext", "caret", "knitr", "rmarkdown"))
     ```

4. **Run the Analysis**
   - Open `AnalysisProject1.Rmd` in RStudio.
   - Click **Knit** to run all the code and generate the full report.
   - This will produce the HTML (or PDF) report with all of our results, including plots, tables, and model outputs.

5. **Troubleshooting**
   - Make sure your working directory is the project folder and the CSV files are in the right place.
   - If anything seems off, you can run `sessionInfo()` in R to check your package versions.



