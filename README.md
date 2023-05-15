# Analysis of Global Suicide Rates

This repository contains a Python script utilized to analyze global suicide rates using data sourced from the World Health Organization (WHO). The script conducts a series of data cleaning, exploratory data analysis, and predictive modeling through linear regression.

## Dataset

The dataset used in this project is accessible on the [World Health Organization website](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/crude-suicide-rates-(per-100-000-population)). 

Key columns in the dataset are: 
- Region
- Country
- Year
- Sex
- Age Range
- Suicide Rate (per 100,000 population)

## Data Processing and Exploratory Data Analysis (EDA)

The script initiates by importing and tidying up the data, which involves renaming columns and discarding the unnecessary ones. Following the data cleaning, an exploratory analysis is conducted to determine the country with the highest and lowest suicide rates, as well as examining the relationship between age groups and suicide rates.

Subsequently, the age ranges are converted to a single age and categorized into 'Adolescent', 'Adults', 'Middle Aged Adults', and 'Elderly'. The association between these age categories and suicide rates is depicted using a bar graph.

The relationship between sex and suicide rate is also investigated, with the results visualized in a bar chart, further broken down by age category.

## Linear Regression Model and Predictive Analysis

The script incorporates a linear regression model to predict suicide rates based on year, sex, and age. The model is trained using a random subset of 80% of the data, with the remaining 20% being used for testing.

The coefficients of the model are evaluated to understand the influence of each feature on the predicted suicide rate. A scatter plot is also generated to illustrate the relationship between age and suicide rate.

## Key Findings

Through the exploratory data analysis and predictive modeling, the script provides insight into the patterns of suicide rates across different countries, age groups, and genders.

## Important Notes

Please ensure to replace the local file path in the `pd.read_csv` function with your own local file path when executing the script.

It should be noted that the correlation coefficient between 'Age' and 'Suicide Rate (per 100,000 population)' was found to be 0.349. This suggests a mild positive linear correlation, implying that as 'Age' increases, 'Suicide Rate (per 100,000 population)' also tends to increase, albeit not strongly or consistently. However, correlation does not imply causation. Even if 'Age' and 'Suicide Rate (per 100,000 population)' are correlated, it doesn't mean that increasing age causes an increase in the suicide rate. Other confounding variables may be influencing this relationship.

## Conclusion

This script provides an initial exploration and analysis of global suicide rates using data from the WHO. The data was tidied and examined to reveal insightful observations. A regression model was also created to predict suicide rates based on year, sex, and age. Further work may delve deeper into the analysis or employ more advanced modeling techniques.
