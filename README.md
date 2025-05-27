**Predicting Titanic Survivors**

This project aims to predict which passengers survived the Titanic disaster using machine learning techniques. The main steps include Exploratory Data Analysis (EDA), Data Preprocessing, Model Building, and Evaluation.

**Exploratory Data Analysis (EDA)**
Explored the dataset to understand the distribution of features.

Identified missing values and how different features relate to survival (e.g., gender, class, family size).



**Data Preprocessing**

1-Ticket Grouping: Grouped passengers by ticket frequency, assuming that families or friends traveling together  (with the same ticket number) have similar survival chances. Dropped the original 'Ticket' feature.

2-Age Imputation: Filled missing 'Age' values with the mean and created a new categorical feature 'Age_Group' (e.g., child,Teen, Young Adult, Adult, Senior). 

3-Family Features: Combined 'SibSp' and 'Parch' to create:

'FamilySize' — total number of family members onboard.

'IsAlone' — a binary feature indicating if the passenger was alone.
Dropped the original 'SibSp' and 'Parch' features.

4-Cabin Feature: Extracted the deck letter from the 'Cabin' feature (e.g., 'C' from 'C85'), as passengers with cabin assignments were more likely to survive. Dropped the original 'Cabin'.

Dropped Unused Features: Removed 'PassengerId' and 'Name' as they are not useful for prediction.



**Model Building**
I Try multiple classification models  like Logistic Regression, Random Forest , XGBoost 


**Evaluation**
I evluate using accuracy, precision, recall, and confusion matrix


