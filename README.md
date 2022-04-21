# SC1015-Data-Science-Project

 # About
 
 Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence), focuses on attrition of employees.
 Dataset obtained from Kaggle, IBM HR Analytics Employee Attrition & Performance by PAVANSUBHASH
 
 For detailed walkthrough, please view the source code in order from:
 1) DataVisualisation.ipynb
 2) DataCleaning.ipynb
 3) MachineLearningModel_(Non_resampled).ipynb
 4) Resampling.ipynb
 5) MachineLearningModel_(resampled).ipynb

#Contributors
- Xcoga
- DivineValleys
- kiannylim

# Problem Definition
- Which factors play a bigger role in determining attrition rates in company (Personal/Workplace)?

# Motivation
Attrition rate is the rate at which people leave the company over time. 
It is a metric that determines how well the company is at retaining employees.
Companies need to retain talents and capable workers in order to maintain functionality and competitiveness with other businesses in the industry.
Hence, we need to know what factors to improve upon in order to retain desirable employees

# Models Used
1) Decision Tree
2) Random Forest Classifier


# Conclusion
- Resampling of dataset using SMOTE() significantly increases performance of decision tree/random forest in predicting "Yes" attrition values
- 'StandardHours','EmployeeCount' and 'Over18', are variables with no deviation. There is no relationship with Attrition.
- 'EmployeeNumber' is an index with no relation with Attrition
- Through Chi Square Test, 'MonthlyIncome','DistanceFromHome','PercentSalaryHike','PerformanceRating',
'YearsSinceLastPromotion' are variables dropped since they are independent on Attrition.
- Random Forest performed consistently well with remaining variables after resampling.
- Feature Importances showed that JobSatisfaction, Age, JobInvolement, TotalWorkingYears and EnvironmentalSatisfaction (in decreasing order) are the top 5 most important features in predicting attrition rates


# What did we learn from this project?
- Handling skewed datasets by using resampling from imblearn packages
- Random Forest Classifier using sklearn.ensemble package
- Using Label Encoding to turn categorical data into integer format using sklearn.preprocessing package
- Using GitHub
- Using contingency Table for chi square test
- Using Chi Square test to find independence of variables to clean data using scipy package
- Converting categorical/numerical columns to a list
- Using cross validation to tune hyperparameters for Random Forest model
- Feature Importance analysis to figure out which variables are the most important in predicting attrition in workers

# References
- https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
- https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/
- https://www.datacamp.com/community/tutorials/random-forests-classifier-python
- https://www.geeksforgeeks.org/contingency-table-in-python/
- https://medium.com/swlh/how-to-run-chi-square-test-in-python-4e9f5d10249d
- https://pbpython.com/categorical-encoding.html
- https://cmdlinetips.com/2020/04/how-to-get-column-names-as-list-in-pandas/
- https://towardsdatascience.com/cross-validation-and-grid-search-efa64b127c1b
- https://mljar.com/blog/feature-importance-in-random-forest/#:~:text=Random%20Forest%20Built%2Din%20Feature%20Importance&text=It%20is%20a%20set%20of,sets%20with%20similars%20responses%20within
