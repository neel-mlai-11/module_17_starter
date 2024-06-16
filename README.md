A Baseline Model
==================================
What is the baseline performance that our classifier should aim to beat? 
Baseline Accuracy (Majority Class Proportion): 0.8873

A Simple Model, Logistic Regression model 
===========================================
Logistic Regression Model Accuracy: 0.9009

Model Comparisons
============================================
Compare the performance of the Logistic Regression model to KNN algorithm, Decision Tree, and SVM models. 

      Model     Train Time   Train Accuracy    Test Accuracy
                 
0  Logistic Regression    0.728165        0.911715       0.911508

1                  KNN    0.170691        0.931745       0.901432

2        Decision Tree    1.012705        1.000000       0.886137

3                  SVM   52.050564        0.925615       0.908352


Improving the Model
=====================================================

More feature engineering and exploration. For example, should we keep the gender feature? Why or why not?
Exploring Gender Feature The dataset doesn't explicitly have a gender feature, but we can consider other features and check their impact.
Hyperparameter tuning and grid search. 
Removing or Modifying Features Based on the dataset description, the 'duration' feature should be removed for a realistic predictive model since it highly affects the output. 
Use GridSearchCV to find the best hyperparameters for each model.

    Model  Train Time  Train Accuracy  Test Accuracy
                 
0  Logistic Regression    0.348226        0.899879       0.897184

1                  KNN    0.154424        0.913596       0.884438

2        Decision Tree    0.779667        0.994143       0.834790

3                  SVM  197.999090        0.901882       0.897791
