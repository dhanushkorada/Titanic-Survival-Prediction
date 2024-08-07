# Titanic Survival Prediction

## Table of Contents

- [Project Overview](#Project-Overview)
- [Dataset](#Dataset)
- [Setup and Installation](#setup-and-Installation)
- [Data Preprocessing](#Data-Preprocessing)
- [Model Selection](#model-selection)
- [Results](#results)
- [License](#license)
- [Acknowledgments](#Acknowledgments)

## Project Overview
This project aims to predict survival outcomes of passengers aboard the Titanic using machine learning techniques. The Titanic dataset is used to train and evaluate various models, with a focus on preprocessing steps and feature engineering to improve prediction accuracy.

## Dataset
The dataset includes the following features:
- `Name`: Passenger's name
- `Ticket`: Ticket number
- `Cabin`: Cabin number
- `PassengerId`: Unique ID for each passenger
- `Survived`: Survival status (0 = No, 1 = Yes)
- `Pclass`: Passenger class (1, 2, 3)
- `Sex`: Gender of the passenger
- `Age`: Age of the passenger
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Fare`: Ticket fare
- `Embarked`: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Setup and Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/dhanushkorada/Titanic-Survival-Prediction.git
    cd Titanic-Survival-Prediction
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Data Preprocessing
- Removed non-informative columns (`Name`, `Ticket`, `Cabin`, `PassengerId`) from the dataset.
- Handled missing values by filling them with appropriate statistics (mean for numerical features, mode for categorical features).
- Applied One-Hot Encoding to convert categorical features into numerical format.
- Scaled the features using `StandardScaler`.

## Model Selection
- Implemented a RBF Kernel SVM to predict survival outcomes.

## Results
- Predictions were made on the test set, and results were saved to `prediction.csv`. The RBF Kernel SVM achieved an accuracy of 78% on the test set.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Dataset: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
