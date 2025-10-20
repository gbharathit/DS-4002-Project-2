# Charlottesville Weather and Review Ratings Project

## Repository Overview
This repository contains all the data, scripts, and output for a project exploring the relationship between historical weather patterns in Charlottesville, VA (2000–2023) and review star ratings. The project includes:  

- Manual extraction and cleaning of NOAA monthly temperature data.  
- Exploratory analysis to identify trends, seasonality, and potential correlation with review ratings.  
- ARIMA time series modeling to forecast 2024 temperatures.  
- Predictive modeling to estimate review star ratings based on temperature trends.  

This repository follows the TIER Protocol 4.0 structure to ensure reproducibility.

---

## Section 1: Software and Platform

**Software Used:**  
- **R Studio** (version X.X.X) for data cleaning, visualization, and modeling.  

**Add-on Packages Used:**  
- `tidyverse`: for data cleaning and manipulation.  
- `forecast`: for ARIMA time series modeling.  
- `ggplot2`: for plotting trends, seasonality, and correlation visualizations.  
- `readr`: for reading CSV files.  

**Platform:**  
- Windows 10  

---

## Section 2: Repository Structure

The repository is organized into four main folders (`SCRIPTS`, `DATA`, `OUTPUT`, and the main README) to match the Protocol.



## Section 2: Repository Structure


---

## Section 3: Instructions for Reproducing Results

1. **Install R and R Studio:**  
   Download and install R from [https://cran.r-project.org](https://cran.r-project.org) and R Studio from [https://www.rstudio.com](https://www.rstudio.com).  

2. **Install required packages:**  
   Open R Studio and run the following commands:
   ```R
   install.packages(c("tidyverse", "forecast", "ggplot2", "readr"))
