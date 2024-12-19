# COVID-19 Statistical Analysis and Dashboard

## Project Overview

This project focuses on performing statistical analysis on COVID-19 data to identify patterns related to race, ethnicity, and gender. The goal is to provide insights on the impact of COVID-19 through **exploratory data analysis (EDA)**, **machine learning models** These insights can help develop targeted strategies for handling future pandemics.

---

## Objectives

1. **Data Analysis**:
   - Analyze COVID-19 death and infection rates by race, ethnicity, and gender.
   - Identify groups most affected by the pandemic.

2. **Visualization**:
   - Compare COVID-19 deaths and cases across different demographics.

3. **Machine Learning**:
   - Implement a **Random Forest** model to predict high/low COVID-19 death rates based on demographic data.

---
## Data Sources

1. **CDC Provisional COVID-19 Deaths by Sex and Age**:
   - [CDC Data Link](https://data.cdc.gov/NCHS/Provisional-COVID-19-Deaths-by-Sex-and-Age/9bhg-hcku)

2. **KFF Population Distribution**:
   - [Population by Age](https://www.kff.org/other/state-indicator/distribution-by-age/)
   - [Population by Sex](https://www.kff.org/other/state-indicator/distribution-by-sex/)

3. **Statista Gender Projections**:
   - [US Population by Gender (2027 Projection)](https://www.statista.com/statistics/737923/us-population-by-gender/)

---

## Methodology

### 1. **Data Import and Cleaning**

- Data imported using `read.table` in R.
- Cleaning steps include renaming columns, removing unnecessary rows, and converting data types.

### 2. **Exploratory Data Analysis (EDA)**

- **Visualizations**:
  - **Stacked Bar Charts** for comparing COVID-19 deaths and cases by race/ethnicity.
  - **Histograms** and **Box Plots** for identifying data distributions and outliers.

### 3. **Machine Learning: Random Forest**

- **Objective**: Predict high/low COVID-19 death rates.
- **Features**:
  - Race/Ethnicity
  - COVID-19 death counts
  - COVID-19 case counts
  - Population demographics
- **Model Evaluation**:
  - **Feature Importance** measured using `MeanDecreaseAccuracy` and `MeanDecreaseGini`.


---

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/covid-statistical-analysis-dashboard.git

   install.packages(c("ggplot2", "dplyr", "randomForest", "reshape", "Metrics"))

Run the R Markdown Script:

Open MILESTONE2_MAHALINGAM.Rmd in RStudio.
Knit the file to generate the analysis report.

Ethical Considerations
Ensured data accuracy and integrity by using trusted sources (CDC, KFF).
Avoided bias by accurately representing demographic data.

References
CDC Data: Provisional COVID-19 Deaths
KFF Data:
Population by Age
Population by Sex
Statista: US Population by Gender

