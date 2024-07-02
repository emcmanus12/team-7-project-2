# team-7-project-2
# INNOVATIVE FEATURE ENGINEERING IN SEATTLE REAL ESTATE
    <"https://img-v2.gtsstatic.net/reno/imagereader.aspx?imageurl=https%3A%2F%2Fsir.azureedge.net%2F1194i215%2Fyxttbmab8sbbmt6hve3xsgzyh2i215&option=N&h=472&permitphotoenlargement=fals">
## Overview

This document outlines the feature engineering process undertaken to enhance the predictive power of our real estate model. The focus has been on incorporating additional features beyond the traditional physical attributes typically considered when purchasing a house.

## New Features Added

1. **Proximity to Employment Centers**:
   - This feature calculates the geographic distance from key employment centers (e.g., Amazon, Starbucks, Nordstrom, Microsoft, Boeing) based on latitude and longitude (as-the-crow-flies distance) rather than commute time. The rationale is that properties closer to major employment hubs tend to command higher prices due to the desirability of shorter commutes.

2. **Urban, Suburban, and Rural Classification**:
   - Properties are classified into urban, suburban, or rural categories. This classification can impact pricing, especially when combined with other factors. It allows the model to differentiate between varying property types and their associated values.

3. **Population Density**:
   - Using an API to retrieve Census data, each property is assigned a population density value. This feature may correlate with the availability of housing and help distinguish between high-density urban areas and less dense suburban areas, both of which can have different pricing dynamics.

4. **Latitude and Longitude Combination**:
   - Latitude and longitude have been combined into a single feature for machine learning purposes. Individually, these coordinates can be misleading; however, combined, they may provide useful information. It should be noted that there is a risk of multicollinearity with the zip code, which will need to be addressed during model validation.

5. **School Districts Classification**:
   - Properties are categorized into eight groups based on the top seven school districts by zip code, with the eighth category encompassing all other properties. This classification recognizes the impact of school district quality on property values.

## Code Setup

- At the beginning of the code, pip imports necessary for a user's conda environment have been included but commented out.
- The setup ensures that no additional encoding is required.

## Conclusion

