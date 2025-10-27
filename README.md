# CaseStudy1DDS
## Executive Summary

This study aims to support Frito-Lay’s Talent Management team by predicting employee attrition — specifically whether an employee is likely to leave the company (“Yes”) or stay (“No”) — using two supervised machine learning models: K-Nearest Neighbors (KNN) and Naive Bayes. Our objective is not only to forecast attrition risk, but to identify which factors most strongly drive turnover so that Frito-Lay can optimize retention strategies and proactively manage talent costs.

Using statistically validated features (Wilcoxon test for numeric variables and Chi-Square test for categorical variables, α = 0.05), we identified the following key drivers influencing attrition: Monthly Income, Distance From Home, Age, Total Working Years, Years at Company, Years in Current Role, and Manager Tenure, along with categorical factors such as Business Travel frequency, Job Role, Job Satisfaction, Overtime status, Marital Status, Environmental Satisfaction, Work-Life Balance, and Department.

After applying SMOTE sampling and training on a 70/30 train-test split, the models achieved the following results:

KNN (k = 65, 0.50 threshold): 62.45% accuracy | 61.90% sensitivity | 62.55% specificity

Naive Bayes (0.75 threshold): 63.60% accuracy | 64.29% sensitivity | 63.47% specificity

While predictive performance was modest, both models showed balanced sensitivity and specificity, confirming that attrition risk is explainable and learnable from employee data. Our primary recommendation is to tune decision thresholds based on whether Frito-Lay prioritizes minimizing turnover cost (higher sensitivity) or avoiding unnecessary retention spending (higher specificity). We further recommend exploring more advanced methods such as ensemble models, gradient boosting, and neural networks to improve predictive accuracy and reduce cost trade offs.

Link To Video Presentation: https://smu365-my.sharepoint.com/:v:/r/personal/ncastellano_smu_edu/Documents/Doing%20Data%20Science/video5235657192.mp4?csf=1&web=1&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=uYz72B
