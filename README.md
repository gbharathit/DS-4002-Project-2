# Charlottesville Weather Forecast Project

This repository contains a dataset of historical weather data for Charlottesville, VA, as well as scripts and outputs to forecast 2024 monthly average temperatures. Our project analyzes trends, seasonality, and anomalies in monthly minimum and maximum temperatures from 2000–2023 using ARIMA modeling. The cleaned dataset, exploratory analyses, and model predictions are included to enable reproduction of all results.

## Contents of this repository
This repository contains everything needed to reproduce the analyses and results for this project: raw and cleaned weather data, R scripts for preprocessing and analysis, output plots, and predicted 2024 temperature data. The sections below outline software requirements, repository structure, and step-by-step instructions to reproduce the results.

---

## Section 1: Software and platform

**Software Used:**
- R Studio (version X.X.X) for data cleaning, exploratory analysis, and ARIMA modeling.
- Git for version control and GitHub for hosting.

**Add-on R Packages Required:**  
Install with `install.packages()` in R if not already installed:  
```R
install.packages(c("tidyverse", "forecast", "ggplot2", "readr", "lubridate"))
