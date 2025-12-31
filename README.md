# NYC Green Taxi Tip Amount Prediction

## Project Overview

This project analyzes NYC Green Taxi trip data from 2018 to predict tip amounts using k-Nearest Neighbors (k-NN) regression. The analysis follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology to understand what factors incentivize passengers to tip cab drivers.

## Business Problem

As a Machine Learning Engineer for the NYC Taxi and Limousine Commission (TLC), this project aims to:
- Analyze where passengers use Green Taxis and how frequently
- Evaluate factors that contribute to drivers receiving tips
- Build a predictive model for tip amounts on future trips

## Dataset

**Source:** NYC Taxi and Limousine Commission (TLC)  
**Data:** Green Taxi Trip Records (2018)  
**Link:** [NYC TLC Trip Record Data](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

The dataset includes:
- Pick-up and drop-off dates/times
- Pick-up and drop-off locations
- Trip distances
- Itemized fares
- Rate types and payment types
- Driver-reported passenger counts

## Methodology (CRISP-DM)

### 1. Business Understanding
- Define the problem: predict tip amounts for Green Taxi trips
- Identify key stakeholders and success metrics

### 2. Data Understanding
- Load and explore the dataset
- Analyze distributions, correlations, missing values, and outliers
- Feature selection: identify predictive variables
- Feature engineering: create new meaningful features (bonus)

### 3. Data Preparation 
- Handle missing data and outliers
- Data transformation and filtering
- Normalization (min-max or z-score standardization)
- Encode categorical variables
- Split data into training and test sets

### 4. Modeling 
- Implement k-NN regression algorithm
- Create `knn.predict()` function
- Calculate Mean Squared Error (MSE)

### 5. Evaluation 
- Test at least 20 different k values
- Visualize k vs. MSE
- Determine optimal k value
- Assess model performance and recommendations

## Requirements

```r
# R Libraries
library(tidyverse)
library(ggplot2)
library(caret)
library(FNN)  # or class package for k-NN
library(dplyr)
library(corrplot)
library(scales)
```

## Project Structure

.
├── README.md
├── Practicum3.Rmd           # Main R Markdown file with analysis
├── Practicum3.html          # Knitted HTML output
├── data/
│   └── green_taxi_2018.csv  # Raw data (not included in repo)
├── figures/                 # Generated visualizations
└── presentation/            # Presentation slides



2. **Download the data:**
   - Download the 2018 Green Taxi data from the [NYC TLC website](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
   - Place the data in the `data/` directory

3. **Install required R packages:**
```r
install.packages(c("tidyverse", "ggplot2", "caret", "FNN", "corrplot"))
```

4. **Run the analysis:**
   - Knit the document to generate the HTML report

## Key Findings

### Data Exploration
- [Describe key patterns found in the data]
- [List correlations with tip amount]
- [Mention any interesting insights]

### Model Performance
- **Optimal k value:** [Your optimal k]
- **Best MSE achieved:** [Your MSE value]
- **Model recommendation:** [Your assessment]

### Visualizations
All charts include:
- Informative titles and subtitles
- Labeled axes with units
- Captions explaining the chart's purpose

## Presentation

A 15-minute presentation summarizing this analysis was delivered on [Date]. The presentation focused on:
- Overall approach and methodology
- Key findings and insights
- Model recommendations
- Business implications

## References

- [NYC TLC Trip Record Data](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- [Data Dictionary](https://www1.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_green.pdf)
- [Normalizing Data with R](https://www.pluralsight.com/guides/normalizing-data-r)
- [k-NN Algorithm Tutorial](https://www.analyticsvidhya.com/blog/2015/08/learning-concept-knn-algorithms-programming/)

