# Health Insurance Premium Prediction
Overview
This project focuses on predicting health insurance premiums for new policy buyers using machine learning techniques. The objective is to build a predictive model based on existing data from an insurance company, taking into account factors such as health, lifestyle, family dynamics, gender, age, and region. The dataset contains information on 1,338 participants.

# Key Steps
Data Exploration: The initial phase involved checking for null values and analyzing numerical features. Outliers were identified in the "BMI" and "Charges" variables, while transformations were applied to normalize the data distribution.

Univariate Analysis: Various visualizations, including pie charts, distribution plots, box plots, and QQ plots, provided insights into the data. Notably, "BMI" conformed to a normal distribution, while "Age" and "Charges" did not. Appropriate transformations were applied, such as Box Cox transformation for "BMI" and Log transformation for "Charges."

Bivariate Analysis: Relationships between variables were explored using box plots and pair plots. Significant insights included the observation that smokers tended to be younger, had fewer children, incurred higher premium charges, and had lower BMIs.

Feature Engineering: Categorical variables ("Sex," "Smoker," and "Region") were encoded for model compatibility.

Assumption Checks: Assumptions of linear regression were assessed. Multicollinearity was detected using Variance Inflation Factor (VIF), and "BMI" was removed from independent variables. A linear relationship was established between "Age" and "Charges." Heteroscedasticity was identified through residual plots, indicating that linear models may not be ideal. Autocorrelation and normality assumptions were met.

# Evaluation Metrics
The data was split into training and test sets.
A regression model was fitted using training data, and the R-squared value for the test data was calculated (0.77).
Cross-validation with k=3 yielded an R-squared value of 0.75, indicating the model's performance.
GitHub ReadMe
This repository contains code and documentation for a health insurance premium prediction project. The project leverages machine learning techniques to predict insurance premiums for new policyholders based on various attributes. Key steps include data exploration, univariate and bivariate analysis, feature engineering, and assumption checks. The model achieved a test R-squared value of 0.77, demonstrating its effectiveness.

For detailed information and code, please explore the repository files.
