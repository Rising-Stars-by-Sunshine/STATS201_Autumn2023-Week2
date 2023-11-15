## Random Forest Code
Referenced based on https://ishanjain-ai.medium.com/understanding-random-forest-algorithm-with-python-code-ae6fb0e34938

The Random Forest algorithm is particularly well-suited for handling nonlinear relationships and complex interactions between features. 
It operates by constructing multiple decision trees during the training phase and outputting the mode of the classes 
(classification) or mean prediction (regression) of the individual trees. Thus, further research can be conducted to test
which variables result with having the chance to have rabies increase or not

## Data Preparation
###Import necessary libraries
import numpy as np
import pandas as pd
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

### Load the dataset
data = load_rabies()
X = pd.DataFrame(data.data, columns=data.feature_names)
y = pd.Series(data.target, name='target')

### Split the dataset into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

## Creating a Random Forest classifier
rf_classifier = RandomForestClassifier(n_estimators=100, max_depth=3, random_state=42)

## Train the classifier on the training data
rf_classifier.fit(X_train, y_train)

## Make predictions on the test data
y_pred = rf_classifier.predict(X_test)

## Calculate accuracy
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy: {accuracy:.2f}")

# Multunomial Naive Bayes Classifier
Referenced based on https://developer.ibm.com/tutorials/awb-classifying-data-multinomial-naive-bayes-algorithm/

Since Naive Bayes Classifier works under the idea that the features are conditionally independent given the output class,
a direct comparison can be made with random Forests.

