Titanic Dataset Analysis README
Overview
This project aims to explore and analyze the Titanic dataset to understand the factors influencing passenger survival. The analysis includes data cleaning, visualization, and extraction of key insights.

File Contents
Titanic_Dataset.ipynb: A Jupyter Notebook containing the Python code for data loading, exploration, visualization, and analysis.

train.csv: The Titanic training dataset used in the analysis.

Data Description
The train.csv dataset contains the following columns:

PassengerId: Unique identifier for each passenger.

Survived: Survival status (0 = No, 1 = Yes).

Pclass: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).

Name: Passenger name.

Sex: Passenger gender.

Age: Passenger age.

SibSp: Number of siblings/spouses aboard.

Parch: Number of parents/children aboard.

Ticket: Ticket number.

Fare: Passenger fare.

Cabin: Cabin number.

Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

Exploration and Analysis
The Jupyter Notebook (Titanic_Dataset.ipynb) performs the following steps:

Data Loading and Inspection:

Imports necessary libraries: pandas, matplotlib.pyplot, and seaborn.

Loads the train.csv dataset into a pandas DataFrame.

Displays the first 10 rows of the dataset using df.head(10).

Data Cleaning:

Handles missing values in the Age, Cabin, and Embarked columns.

Prints the count of missing values for each column using df.isnull().sum().

Fills the missing values in the Age column with the median age.

Fills the missing values in the Embarked column with the mode.

Drops the Cabin column due to a large number of missing values.

Descriptive Statistics:

Generates descriptive statistics for numerical columns using df.describe().

Provides summary statistics such as count, mean, standard deviation, minimum, and maximum values.

Data Visualization:

Generates a scatter plot of Age vs. Fare, with points colored by survival status.

Key Findings from the Scatter Plot
Passengers who paid higher fares generally had a higher chance of survival (purple points tend to concentrate at higher fare values).

There is a dense cluster of passengers with lower fares, and a mix of survival outcomes within this group.

Some passengers in the younger age groups had higher survival rates. This might be due to prioritization in rescue efforts.

There are a few outliers of passengers who paid very high fares, and most of them survived.
