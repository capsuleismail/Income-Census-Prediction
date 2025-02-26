## Introduction  
---------------

The Adult Census UCI dataset, commonly referred to as the Adult dataset, is a well-known dataset from the UCI Machine Learning Repository. It is widely used for classification tasks in machine learning and data science. With multiple missing values, this dataset provides a valuable opportunity to analyze and compare the effectiveness of different algorithms, helping to understand why one may be more suitable than another. In this case I used XGBoost for its quality such as fast, robust and capable to handle missing values. 

**Purpose:** Predict whether a person earns more than $50K per year based on demographic and employment-related attributes.<br/>
**Source:** Extracted from the 1994 U.S. Census Bureau data.<br/>
**Common Usage:** Used for classification models, such as logistic regression, decision trees, and neural networks. In this case I used XGBoost for is advantages such as fast and capable to handle missing values.<br/>

These are the questions I've gone through on my notebooks:

1. **Density and Outliers detection.** <br/>
2. **What is the gender distribution in the dataset?** <br/>
3. **What are the most common education levels?** <br/>
4. **How is the relationship between age and hours-per-week?** <br/>
5. **Which work classes are most represented, and how do they vary by gender?** <br/>
6. **What is the proportion of individuals earning more than $50K?** <br/>
7. **Is there a relationship between education level and income?** <br/>
8. **Does marital-status affect the income?** <br/>
9. **What is the relationship between hours worked per week and income?** <br/>
10. **Which occupation types are most associated with earning more than $50K?** <br/>
11. **Which countries have the highest percentage of individuals earning more than $50K?** <br/>
12. **Are there any differences in income levels between different races?** <br/>
13. **Modeling with XGBClassifier.** <br/>
14. **XGBClassifier Cross Validation with StratifiedKFold on 10 splits.**
15. **XGBClassifier with ConfusionMatrixDisplay plot.** <br/>


**Citation: [The Adult Census UCI dataset]([https://archive.ics.uci.edu/dataset/942/rt-iot2022](https://archive.ics.uci.edu/dataset/2/adult)). (1994). UCI Machine Learning Repository.** <br/>
--------------------------------------------------------------------------------------------------------------------


### I. How to import the dataset via pip.
--------------------------------------------------------------------------------------------------------------------
```
!pip install ucimlrepo
from ucimlrepo import fetch_ucirepo 
  

adult = fetch_ucirepo(id=2) 
  

X = adult.data.features 
y = adult.data.targets 
  

print(adult.metadata) 
  

print(adult.variables)
```
--------------------------------------------------------------------------------------------------------------------

