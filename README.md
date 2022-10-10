# Credit Risk Analysis

# Overview of the loan prediction risk analysis:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Jill a client asks me to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. 

First the steps were to Read the CSV and Perform Basic Data Cleaning and then Split the Data into Training and Testing. We named the new data clean_loans.csv.

The next steps were to create Six Machine Learning Models with Oversampling, SMOTE Oversampling, Undersampling(Cluster Centroids), Combination (Over and Under) Sampling (SMOTEEN), and our two Ensemble Learners (Balanced Random Forest Classifier and Easy Ensemble Classifier)




Here is the results...

# Results:

## Six Machine Learning Models

### RandomOverSampler

![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Oversampling_Oversampling_confusion_matrix.png)

* Accuracy Score: 83.25% (0.8325468421491353)

* Confusion Matrix: <br> 
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Oversampling_Oversampling_confusion_matrix.png)

* Imbalanced Classification Report: <br> 
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/random_oversampling_icr.png)

### SMOTE

* Accuracy Score: 84.40% (0.8440938486973113)

* Confusion Matrix:<br> 
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling_confusion_matrix.png)

* Imbalanced Classification Report:<br> 
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/SMOTE_inbalanced_classification_report.png)

### Cluster Centroids (Undersampling)

* Accuracy Score: 84.40% (0.8440938486973113)

* Confusion Matrix:<br> 
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_confusion_matrix.png)

* Imbalanced Classification Report:<br> 

![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Undersampling_inbalanced_classification_report.pnng.png)



## Use the SMOTEENN algorithm to Predict Credit Risk

SMOTEEN Algorithm

* Accuracy Score: 84.40% (0.8440938486973113)

* Confusion Matrix:<br>
Combination (Over and Under) Sampling

![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Combination_Over_and_Under_Sampling_confusion_matrix.png)

* Imbalanced Classification Report:<br>
![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Combination%20(Over%20and%20Under)%20Sampling_inbalanced_classification_report.png)


## Use Ensemble Classifiers to Predict Credit Risk


### BalancedRandomForestClassifier

* Accuracy Score: 75.9% (0.759)

Included below:

* Confusion Matrix:

* Imbalanced Classification Report:

![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest_Classifier_jupyter_notebook.png)

### EasyEnsembleClassifier

* Accuracy Score: 93.19% (0.9319231677611166)

Included below:

* Confusion Matrix:

* Imbalanced Classification Report:

![This is an image](https://github.com/ABorden23/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier_jupyer_notebook.png)

# Summary:

As far as the Six Machine Learning models we created Random Sampler scored 83.25%, our SMOTE scored 84.40% and Cluster Centroids (Undersampling) scored a 84.40%.

The EasyEnsembleClassifier performed the best with a Accuracy Score of 93.19% (0.9319231677611166). The EasyEnsembleClassifier would be my recommendation on which model to using Ensemble Classifiers. 



 ### Machine Learning Libraries Used:

* scikit-learn
* imbalanced-learn

### Software Used:

* Jupyter Notebook
* VS Code
