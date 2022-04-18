# SC1015-Data-Science-Project

 # About
 
 Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence), focuses on attrition of employees.
 For detailed walkthrough, please view the source code in order from:
 
 1) Data Extraction
 2) Data Visualisation
 3) Data Resampling and Splitting
 4) Decision Tree
 5) Random Forest Classifier

#Contributors
- Xcoga
- DivineValleys
- kiannylim

# Problem Definition
- How should we predict the attrition rate of employee based on workplace/personal factors?

# Motivation
In a competitive job landscape, what should companies do in order to retain talented or desirable workers?

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


# What did we learn from this project?
- Handling skewed datasets by using resampling from imblearn packages
- Random Forest Classifier using sklearn.ensemble package
- Using Label Encoding to turn categorical data into integer format using sklearn.preprocessing package
- Using GitHub
- Using contingency Table for chi square test
- Using Chi Square test to find independence of variables to clean data using scipy package
- Converting categorical/numerical columns to a list
- Using cross validation to tune hyperparameters for Random Forest model

# References
- https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/
- https://www.datacamp.com/community/tutorials/random-forests-classifier-python
- https://www.geeksforgeeks.org/contingency-table-in-python/
- https://medium.com/swlh/how-to-run-chi-square-test-in-python-4e9f5d10249d
- https://pbpython.com/categorical-encoding.html
- https://cmdlinetips.com/2020/04/how-to-get-column-names-as-list-in-pandas/
- https://towardsdatascience.com/cross-validation-and-grid-search-efa64b127c1b
