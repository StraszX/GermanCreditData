# German Credit Risk Analysis with Logistic Regression

# Overview
This project involves a detailed analysis of the South German Credit dataset, aiming to predict credit risk based on various financial and personal attributes. Using R and several packages like MASS, tidyverse, ggplot2, pROC, dplyr, and scales I conducted exploratory data analysis (EDA), visualized key variables, and developed a logistic regression model to assess the likelihood of credit risk.


# Data Preparation
The dataset was first cleaned and preprocessed, including renaming variables for better readability and converting categorical variables and binary outcomes to the correct format. For instance, CreditRisk was transformed to have labels "Good" and "Bad", facilitating intuitive analysis and visualization.


# Exploratory Data Analysis (EDA)
In this comprehensive analysis, I delved into the dataset to uncover insights and patterns related to credit risk. Initial visualizations, including the distribution of credit risk, histograms of age, and scatter plots of credit amount vs. age, revealed key characteristics of the dataset. These visual explorations highlighted a potential model bias due to an imbalance in the target variable, as well as significant relationships between age, credit amount, and credit risk status.

To further enrich the analysis, I incorporated dark theme settings across all visualizations, enhancing the clarity and aesthetic appeal of the plots. This thematic consistency ensures an engaging and visually cohesive presentation of the findings.


# Categorical Variable Distribution Analysis
A series of bar plots were generated to explore the distribution of various categorical predictor variables by credit risk status, including CheckingAccountStatus, Duration, CreditHistory, Purpose, Savings, InstallmentRate, Housing, and ForeignWorker. Each plot highlights the count of observations for the categories within these variables, distinguished by credit risk status ("Good" vs. "Bad"). This analysis offers a nuanced understanding of how different factors relate to credit risk.

# Credit Amount Summary by Credit Risk
A detailed summary of CreditAmount for "Good" (0) and "Bad" (1) credit risks was conducted, calculating the mean, median, minimum, and maximum credit amounts within each group. This summary provides a deeper insight into the financial behavior associated with each credit risk category.

The visualization of these summaries employs a dark theme, with distinct color coding (green for "Good" and red for "Bad") to delineate between the credit risk categories. Point markers indicate mean and median values, while segments represent the range from minimum to maximum credit amounts. This visual representation underscores the differences in credit amount distributions across the risk categories, aiding in the identification of trends and outliers.


# Model Development
A full logistic regression model was built using all available predictors, followed by stepwise regression to identify a reduced model with significant predictors. The reduced model focused on variables like CheckingAccountStatus, Duration, CreditHistory, Purpose, and Age, among others.


# Model Interpretation
The logistic regression model provided coefficients for each predictor, quantifying their impact on the probability of being classified as "Bad" credit risk. For example, higher values in CheckingAccountStatus and certain Purpose categories significantly increased the risk, while longer Duration and higher CreditAmount had a minimal negative impact.


# Model Evaluation
The model's performance was evaluated using the Area Under the Curve (AUC) metric from the Receiver Operating Characteristic (ROC) curve, indicating its ability to discriminate between good and bad credit risks effectively. A detailed mathematical equation of the logistic regression model was also derived, illustrating the log odds of the outcome as a function of the predictors.


# Conclusion
The logistic regression analysis highlighted key factors influencing credit risk, providing valuable insights for financial institutions in assessing creditworthiness. The model's coefficients and AUC demonstrated its predictive power, though further validation and refinement could enhance its application in real-world scenarios.


# Repository Content
This repository includes all R scripts used for data preprocessing, EDA, model building, and evaluation, alongside a detailed R Markdown report summarizing the methodology, findings, and interpretations.
