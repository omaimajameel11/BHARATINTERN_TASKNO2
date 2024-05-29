# BHARATINTERN_TASKNO2

## Titanic Classification

This project focuses on building a predictive model to determine the likelihood of survival for passengers on the Titanic. We will use data science techniques, including data preprocessing, feature engineering, and machine learning, to achieve this goal.

## Project Structure

```
titanic_survival_prediction/
│
├── data/
│   └── titanic.csv             # Dataset containing Titanic passenger data
│
├── src/
│   ├── data_preprocessing.py   # Script for data cleaning and preprocessing
│   ├── feature_engineering.py  # Script for feature engineering
│   ├── model_training.py       # Script for training the model
│   └── evaluate_model.py       # Script for evaluating the model
│
├── README.md                   # This README file
│
├── requirements.txt            # Python dependencies
│
└── run.py                      # Main script to run the entire pipeline
```

## Dependencies

The project requires the following Python packages:

- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- 
## Features for Titanic Classification

For predicting the likelihood of survival for passengers on the Titanic, we need to extract and engineer meaningful features from the dataset. Here are the key features we will use:

## 1. Data Preprocessing

Before feature extraction, we need to preprocess the data. This involves:
- Handling missing values
- Encoding categorical variables
- Normalizing numerical variables

## 2. Feature Engineering

## 2.1. Basic Features

- **Pclass**: Passenger class (1st, 2nd, 3rd)
- **Sex**: Gender of the passenger (male, female)
- **Age**: Age of the passenger
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Fare**: Ticket fare paid by the passenger
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## 2.2. Derived Features

- **FamilySize**: Total number of family members aboard (SibSp + Parch + 1)
- **IsAlone**: Indicator if the passenger was alone (1 if FamilySize == 1, else 0)
- **Title**: Extracted title from passenger names (e.g., Mr, Mrs, Miss, etc.)
- **FarePerPerson**: Fare divided by FamilySize
- **AgeGroup**: Categorical age group (e.g., Child, Teen, Adult, Senior)
- **Deck**: Deck information extracted from the cabin number
- **TicketPrefix**: Prefix of the ticket number

In this implementation:
- We preprocess the data by filling missing values and encoding categorical variables.
- We engineer additional features like `FamilySize`, `IsAlone`, `Title`, `FarePerPerson`, `AgeGroup`, `Deck`, and `TicketPrefix`.
- We train a Random Forest model on the engineered features and evaluate its performance.

These features provide a robust foundation for predicting the likelihood of survival for Titanic passengers. 
