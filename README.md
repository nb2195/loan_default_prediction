# Loan Default Prediction

This program is intended to predict if a Bank loan has turned bad or is still in the good books. The program makes use to a Decision Tree Classifier model and a Logistic Regression Model to make predictions.

## Tech-stack

1. Python \
    a. Pandas - for reading the dataset into a pandas dataframe\
    b. PySpark - for reading the input data into a Spark Dataframe in order to run Machine Learning models on the same\
    c. PySpark MLLib - for training, testing and making predictions by employing ML models\
    d. pandas-profiling - for exploratory data analysis

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install PySpark, pandas and pandas-profiling.

```bash
pip install pyspark, pandas==1.2.1, pandas-profiling==2.7.1
```

## Python(ipynb) files description
1. PySpark_MLLib.ipynb
    >This program creates the spark session and reads the input file. Post that it splits the data into 2 chunks - train and test, in order to train the ML model. Finally it saves the trained ML model on a persistent storage - google drive in this case.

    >The program generates 2 ML Models - Decision Tree Classifier and Logistic Regression

2. Decision_Tree_Classifier_Model.ipynb
    >This program reads the input and the trained DT model. Post that it generates predictions on the read dataset

3. Logistic_Regression_Model.ipynb
    >This program reads the input and the trained LR model. Post that it generates predictions on the read dataset

4. Pandas-Profiling.ipynb
    >This program reads the input file and generates pandas-profile report for exploratory data analysis