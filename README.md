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
1. DataFolder
AverageTemps.csv – Full dataset with months and years, as well as the mean maximum and minimum temperature values used in analysis. <br>
Metadata.md – Metadata description file. <br>
mean_max_monthly_temps_2000_2025.csv – Just the mean maximum monthly temperature data. <br>
mean_min_monthly_temps_2000_2025.csv – Just the mean mimimum monthly temperature data. <br>
2. OUTPUT
1jantrends.png – Scatter plot with line of best fit of the mean minimum and maximum temperatures in January from 2000-2025. <br>
2juntrends.png – Scatter plot with line of best fit of the mean minimum and maximum temperatures in June from 2000-2025. <br>
3maxtimeseries.png – Decomposition of the additive time series of our maximum temperature data, which shows seasonal and nonseasonal trends. <br>
4mintimeseries.png – Decomposition of the additive time series of our minimum temperature data, which shows seasonal and nonseasonal trends. <br>
6ModelPDF.pdf – Full project analysis for building time series model with minimum and maximum temperature data. <br>
3. SCRIPTSFolder
Data Cleaning.Rmd – Data cleaning script where data is joined as well as general cleaning as well creation of EDA plots.<br>
Model Building.Rmd – Model building script where time series model is fitted. <br>


## Section 3 – How to Reproduce Our Results


