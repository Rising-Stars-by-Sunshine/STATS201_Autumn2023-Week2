## Necessary Code from Lee's Research
Following the step-by-step procedure shared in Lee's GitHub page:

- [x] Install the dependencies.
* LanguageModel.py
* classifier_m.py
* features.py
* driver_m.py
* subject_object_extraction.py

## Why Random Forest

With Lee mentioning the use of the decision tree, Shide and Patil emphasized that "decision tree is over-fitting which can be handled by employing Random Forest. Ensemble of trees has led to considerable enhancement in the accuracy of the classification and permitted to vote for most accepted class" (Shinde & Patil, 2023). Following, with other researchers, including Shide and Patil, found that Random Forrest was proven to be the most accurate, my hypothesis was raised (Dewi & Imah, 2020; Qureshi et al., 2023).

Shinde, A. V., &amp; Patil, D. D. (2023). A multi-classifier-based recommender system for early autism spectrum disorder detection using machine learning. Healthcare Analytics, 4, 100211. https://doi.org/10.1016/j.health.2023.100211 

## What is Random Forest

The Random Forest algorithm is particularly well-suited for handling nonlinear relationships and complex interactions between features. 
It operates by constructing multiple decision trees during the training phase and outputting the mode of the classes 
(classification) or mean prediction (regression) of the individual trees.

## Random Forest's Code
Referenced based on https://ishanjain-ai.medium.com/understanding-random-forest-algorithm-with-python-code-ae6fb0e34938

### Import necessary libraries
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

### Creating a Random Forest classifier
rf_classifier = RandomForestClassifier(n_estimators=100, max_depth=3, random_state=42)

### Train the classifier on the training data
rf_classifier.fit(X_train, y_train)

### Make predictions on the test data
y_pred = rf_classifier.predict(X_test)

## Calculate accuracy
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy: {accuracy:.2f}")

# Multunomial Naive Bayes Classifier
Referenced based on https://developer.ibm.com/tutorials/awb-classifying-data-multinomial-naive-bayes-algorithm/

Since Naive Bayes Classifier works under the idea that the features are conditionally independent given the output class,
a direct comparison can be made with random Forests.

## What more needed
With using the Random Forest, parameter setting would be necessary to better tailor the algorithm to our research. Thus, by following the basic idea given from
### Shide and Patil's Instructions on using Random Forest
1. Choose random data samples from the training dataset
2. Construct the decision tree using chosen data samples
3. Select the number of decision trees to be built.
4. On arrival of new data sample, Classifier predicts final decision using majority of votes given by decision-constructed trees.

### Lee's Markdown on Decision Tree's Parameter Setting (
1. Criterion - the function that measures the quality of a split. Criterion functions
tested are the Gini impurity and entropy information gain.
2. Splitter - the strategy used to select a split point at each node. Available options
are random or best split.
3. Max features - the number of features considered when looking for the best split.
Options tested are log2(n features), sqrt(n features) and n features.
4. Max depth - the maximum
* Optimal parameters for the decision tree are: criterion = entropy, splitter = best split, max features = sqrt(n features) and max depth = 10.
