# Titanic Survival Prediction Project

This project focuses on predicting the survival of passengers on the Titanic using machine learning. The dataset used is the famous Titanic dataset, which provides information about passengers such as age, sex, class, and whether they survived or not.

## Project Description

The goal of this project is to build and evaluate a classification model to predict whether a passenger survived (Survived = 1) or not (Survived = 0). The workflow includes data preprocessing, feature engineering, and the use of machine learning algorithms to achieve the best performance.

## Dataset

The dataset used in this project comes from the Titanic competition on Kaggle. It contains the following key features:
- *Pclass*: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).
- *Sex*: Gender of the passenger.
- *Age*: Age of the passenger.
- *SibSp*: Number of siblings/spouses aboard.
- *Parch*: Number of parents/children aboard.
- *Fare*: Fare paid for the ticket.
- *Embarked*: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).
- *Survived*: Target variable (0 = No, 1 = Yes).

## Methodology

### 1. Data Preprocessing
- Missing values in Age were filled using the mean value grouped by Sex and Pclass.
- The Embarked column was imputed with the mode.
- Categorical variables (Pclass, Sex, Embarked) were encoded using *Label Encoding*.

### 2. Feature Engineering
- The dataset was split into training and testing sets using an 80/20 split.
- Numerical features (Age, Fare) were scaled using *StandardScaler* to normalize the data.

### 3. Model Training
- The primary model used was a *Random Forest Classifier*, which is well-suited for this type of tabular data.

### 4. Model Evaluation
- Accuracy was used as the primary metric to evaluate model performance.
- Other metrics such as *Precision, **Recall, **F1-Score, and **ROC-AUC* were computed for a more comprehensive evaluation.

## Results

The Random Forest model achieved an accuracy of approximately *81%* on the test set. Further improvements could involve additional feature engineering or experimenting with hyperparameter tuning.
