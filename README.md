# INNOVATIVE FEATURE ENGINEERING IN SEATTLE REAL ESTATE

## Overview

This document outlines the feature engineering process undertaken to enhance the predictive power of our real estate model. The focus has been on incorporating additional features beyond the traditional physical attributes typically considered when purchasing a house.

# Objective
The primary objective of this project is to display advanced data analysis and advance data cleaning techniques for machine learning models to extract predictive features from real estate data. By doing so, we aim to provide techniques and tools necessary to make data-driven decisions to optimize investments, and real estate strategies.

# Data analysis and Feature Engineering Data to Optimize ML Predictions from Real Estate Data

1. Data Loading and Cleaning: Importing real estate datasets and performing thorough data cleaning to ensure accuracy and reliability.
2. Feature Engineering: Creating and optimizing features such as living_to_lot_ratio to enhance model performance and provide deeper insights.
3. Outlier Detection: Identifying and analyzing outliers to understand anomalies and their impact on the real estate market.
4. Multicollinearity Analysis: Addressing multicollinearity in features to improve model robustness and interpretability.
5. Model Training and Evaluation: Training various machine learning models, including Gradient Boosting, Random Forest, and KNN, and evaluating their 
   performance.
6. Hyperparameter Tuning: Using techniques such as Grid Search to find the best model parameters for optimal performance.
7. Prediction and Sensitivity Analysis: Making predictions on real estate prices and conducting sensitivity analysis to understand the impact of 
   different features.
8. Visualization: Creating visual representations of data and model results to facilitate better understanding and communication of insights.

## The Engineered Features Added

### 1. Proximity to Employment Centers
![Proximity to Employment Centers](images/employment_centers.png)
   - This feature calculates the geographic distance from key employment centers (e.g., Amazon, Starbucks, Nordstrom, Microsoft, Boeing) based on latitude and longitude (as-the-crow-flies distance) rather than commute time. The rationale is that properties closer to major employment hubs tend to command higher prices due to the desirability of shorter commutes.

### 2. Urban, Suburban, and Rural Classification
![Urban, Suburban, and Rural Classification](images/classification.png)
   - Properties are classified into urban, suburban, or rural categories. This classification can impact pricing, especially when combined with other factors. It allows the model to differentiate between varying property types and their associated values.

### 3. Population Density
![Population Density](images/population_density.png)
   - Using an API to retrieve Census data, each property is assigned a population density value. This feature may correlate with the availability of housing and help distinguish between high-density urban areas and less dense suburban areas, both of which can have different pricing dynamics.

### 4. Latitude and Longitude Combination
![Latitude and Longitude Combination](images/lat_long_combination.png)
   - Latitude and longitude have been combined into a single feature for machine learning purposes. Individually, these coordinates can be misleading; however, combined, they may provide useful information. It should be noted that there is a risk of multicollinearity with the zip code, which will need to be addressed during model validation.

### 5. School Districts Classification
![School Districts Classification](images/school_districts.png)
   - Properties are categorized into eight groups based on the top seven school districts by zip code, with the eighth category encompassing all other properties. This classification recognizes the impact of school district quality on property values.

# Benefits

1. Informed Decision-Making: Utilize AI data-exploration techniquest to get insights for Real estate decisions, reducing risks and maximizing returns on investments.
2. Enhanced Strategies: Develop and refine real estate strategies based on comprehensive data analysis and predictive modeling.
3. Innovative AI Solutions: Explore and implement innovative AI enhancements to stay ahead in the competitive real estate market.
4. Wide Applicability: Whether you are involved in commercial real estate, residential properties, or family investments, this project provides 
   valuable tools and knowledge applicable to all.

## Code Setup

- At the beginning of the code, pip imports necessary for a user's conda environment have been included but commented out.
- The setup ensures that no additional encoding is required.

## Conclusion
This project is a testament to the power of data and AI in transforming the real estate industry. By harnessing the insights and tools provided here, entrepreneurs, investors, and families can make smarter decisions and achieve greater success in their real estate endeavors. We hope this project inspires you to explore the endless possibilities that data analysis and AI offer for the future of real estate. **120 min Run Time Estimate 

