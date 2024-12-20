# Effect of Property Features on Real Estate Prices in Ames, Iowa

## Overview
This project analyzes the Ames Housing dataset to understand various factors influencing house prices in Ames, Iowa. The analysis covers property features, seasonal influences, and neighborhood characteristics using data from 2,930 residential sales between 2006 and 2010.

## Key Findings
- Overall quality and total area are the strongest predictors of sale price
- Newer homes generally command higher prices, with age showing a negative correlation with sale price
- Remodeled homes sell for more across all age categories
- The Random Forest model outperformed linear regression in predicting house prices
- Location and zoning classification significantly impact property values
- Luxury features like pools and fireplaces show mixed effects on sale prices

## Models and Performance
Two predictive models were developed and compared:

1. Linear Regression Model
   - RMSE: 35,084.12
   - R-squared: 0.7748
   - Key predictors: Overall Quality, Total Area, Age at Sale

2. Random Forest Model
   - RMSE: 30,958.19
   - Better performance in handling non-linear relationships
   - More robust to outliers

## Key Variables Analyzed
- Overall Quality Rating
- Total Area
- Age at Sale
- Number of Bathrooms
- Remodeling Status
- Seasonal Effects
- Central Air Conditioning
- Location Specifics

## Technical Details
- Language: Python
- Libraries Used:
  - Pandas for data manipulation
  - Matplotlib/Seaborn for visualization
  - Scikit-learn for modeling

## Data Preprocessing Steps
1. Handled missing values through:
   - Removal of columns with >50% missing data
   - Median imputation for numerical features
   - Mode imputation for categorical features
2. Feature engineering:
   - Created new variables like TotalArea and AgeAtSale
   - Encoded categorical variables
   - Removed multicollinear features

## Visualizations Include
- Distribution of sale prices
- Correlation matrix of key variables
- Seasonal price trends
- Quality vs. price relationships
- Area vs. price analysis
- Age effects on property values

## Future Improvements
1. Feature Engineering:
   - Develop more complex derived variables
   - Incorporate additional neighborhood characteristics

2. Model Optimization:
   - Hyperparameter tuning
   - Exploration of other algorithms
   - Better handling of outliers

3. Data Enhancement:
   - Include more recent data
   - Add external economic indicators
   - Incorporate market trend data
