# Solar Power Plant Generation Prediction

## Overview

This repository contains code and documentation for predicting solar power generation at two plants, Gandikota and Nashik, based on weather data. The goal is to create accurate predictions for daily power output using machine learning models.

## Data Sources

The data used in this project is sourced from Kaggle.org and OpenWeatherMap.org. It includes information on power generation and weather conditions over a 34-day period.

## Problem Statement

Solar power plants face the challenge of unpredictability. The goal is to use data to better predict the output of a solar power plant on any given day, considering individual arrays and the overall plant performance.

## Approach

1. **Data Wrangling:**
   - Merged weather and power datasets.
   - Handled missing data by converting to null values.

2. **Exploratory Data Analysis:**
   - Identified outliers in power generation data.
   - Introduced Nominal Operating Cell Temperature (NOCT) as a metric.

3. **Pre-Processing and Training Data:**
   - Found coefficients between variables.
   - Used equations to convert temperature and irradiation to power output.
   - Tested equations with simple linear regression.

4. **Modeling:**
   - Tested three models: Linear Regression, Random Forest, and Gradient Boosting.
   - Selected Gradient Boosting as the most accurate prediction model.

5. **Prediction:**
   - Combined NOCT equation with coefficients to find a predicted sum.
   - Tested model performance with random data.

6. **Weather Data Prediction:**
   - Used meteorological data from Gandikota for the past 20 years.
   - Calculated yearly power generation and predicted the trend for 2021.

7. **Conclusion:**
   - Highlighted the importance of machine learning in making accurate predictions.
   - Explored the potential benefits of upgrading solar arrays based on industry averages.
