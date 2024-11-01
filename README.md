<h1> Predicting Health Life Expectancy Using ML Models </h1>

<h2> Overview </h2>
This project aims to analyze and predict "Healthy Life Expectancy at Birth" using 
various socio-economic and health-related indicators. The data, sourced from the 
World Happiness Report (WHR) 2018, includes metrics such as GDP, social support, and 
freedom levels from multiple countries. Through data preprocessing and feature 
selection, multiple regression models, including Linear Regression and Decision Tree Regression,
are implemented to predict life expectancy. The findings provide insights into the influence
of specific indicators on life expectancy across countries.

<h2> Objectives </h2>

- **Data Exploration**: Gain insights into the WHR data, examining key descriptive statistics
and identifying relevant features for analysis.
- **Predicting Modelling**: Build and evaluate models to predict "Healthy Life Expectancy at Birth"
using a variety of subjective indicators.
- **Feature Importance Analysis**: Identify the impact of individual features on life expectancy
to understand which socio-economic factors most strongly influence it.
- **Performance Evaluation**: Compare model accuracies, using RMSE as the primary metric, to select the most
reliable predictive model

<h2> Methodology </h2>

1. Preprocessing: Loaded WHR dataset, conducting initial inspections with Dataframe .head() and .describe(),
   cleaned data by removing irrelevant columns (e.g. year, GINI indices..), grouped data by country, split data
   into features X and target variable y.
   
3. Modelling Approach:
   - Linear Regression: Standardized data with StandardScaler, trained model, evaluated performance with RMSE
   - Decision Tree Regression: Utilized regressor on raw data (perks of a DT), evaluated performance with RMSE
    
4. Visualization: Visualized with Matplotlib, creating a bar chart for each model

<h2> Results/Key Findings </h2>

**Model performance**: Linear regression and DT regressive models both performend with RMSE of 2-5 years.

**Feature performance**: LR revealed the importance weights, DT revealed which factors are most decisive such as GDP
and most interestingly, the *Life Ladder*, a personal subjective measurement of life satisfiability 

<h2> Notes </h2>

- In the future, I will consider using Random Forest to improve accuracy
- Could've explored using a neural network to handle non-linear relationships
- Expanding scope of data to more recent (e.g. 2024) or during important events (e.g. 2020 COVID) could
  reveal interesting shifts of feature weights and predictions 
