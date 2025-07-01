# Titanic Survival Prediction Project

This project focuses on predicting the survival of passengers on the Titanic using machine learning. The dataset used is the famous Titanic dataset, which provides information about passengers such as age, sex, class, and whether they survived or not.

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

## Methodology and Results

The methodology that has been followe is: 
- 1. Data Preprocessing: the unuseful data is removed and the null values are corrected. 
- 2. Feature Engineering: the data is splitted into categorical variables (Pclass, Sex, Embarked), encoded using *Label Encoding*, and numerical variables (Age, Fare), scaled using *StandardScaler* to normalize the data.
- 3. Model Training: the primary model used was a *Random Forest Classifier*, which is well-suited for this type of tabular data.

The Random Forest model achieved an accuracy of approximately *81%* on the test set. Further improvements could involve additional feature engineering or experimenting with hyperparameter tuning.

## Requirements

To run the notebook, the following Python libraries are required:

* `numpy`
* `pandas`
* `scikit-learn`
* `jupyter`

Install them using:

```bash
pip install numpy pandas scikit-learn jupyter
```

## How to Use

Clone the repository:

```bash
git clone https://github.com/JoseCDS17/CosmologicalPerturbations-TFG.git
cd CosmologicalPerturbations-TFG
```