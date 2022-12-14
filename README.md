# Credit Risk Analysis

### Deliverable 1: Use Resampling Models to Predict Credit Risk  
This section presents an analysis of each of the following algorithms:
#### ⚫ Naïve Random Oversampling
#### ⚫ SMOTE Oversampling
#### ⚫ Undersampling with ClusterCentroids
Below are screenshots showing the following results of each of the algorithms:
#### Naïve Random Oversampling: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![Naive_Random_Oversampling.png](Resources/Naive_Random_Oversampling_2.png)
#### SMOTE Oversampling: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![SMOTE_Oversampling.png](Resources/SMOTE_Oversampling_2.png)
#### Undersampling with ClusterCentroids: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![Undersampling.png](Resources/Undersampling_2.png)
### Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
This section presents an analysis of the Combination (Over and Under) Sampling algorithm, also known as the <b>SMOTEENN</b> algorithm. Below is a screenshot of the results:
#### Combination (Over and Under) Sampling: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![Combination_(Over_and_Under)_Sampling.png](Resources/Combination_(Over_and_Under)_Sampling_2.png)
### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
This section presents an analysis of each of the following ensemble classifiers:
#### ⚫ Balanced Random Forest Classifier
#### ⚫ Easy Ensemble AdaBoost Classifier
Below are screenshots showing the following results of each of the algorithms:
#### Balanced Random Forest Classifier: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![Balanced_Random_Forest_Classifier.png](Resources/Balanced_Random_Forest_Classifier_2.png)
#### Features sorted in descending order by feature importance
![Balanced_Random_Forest_Classifier_sorted.png](Resources/Balanced_Random_Forest_Classifier_sorted_2.png)
#### Easy Ensemble AdaBoost Classifier: Accuracy Score, Confusion Matrix, and Imbalanced Classification Report
![Easy Ensemble AdaBoost Classifier.png](Resources/Easy_Ensemble_AdaBoost_Classifier.png)
### Deliverable 4: Written Report on the Credit Risk Analysis

The purpose of this analysis is to evaluate several machine learning models by using resampling models and ensemble classifiers to determine which models are best at predicting credit risk.

Resampling models include the following:

#### ⚫ Naïve Random Oversampling
#### ⚫ SMOTE Oversampling
#### ⚫ Undersampling with ClusterCentroids
#### ⚫ Combination (Over and Under) Sampling, a.k.a. SMOTEENN

Ensemble classifiers include the following:

#### ⚫ Balanced Random Forest Classifier
#### ⚫ Easy Ensemble AdaBoost Classifier

This portion of the report presents balanced accuracy scores and the precision and recall scores of all six machine learning models, with screenshots of of the outputs to support the results.

Here is a table showing the balanced accuracy scores of each model, or simply the percentage of predictions that are correct:

![Accuracy_Score_Table.png](Resources/Accuracy_Score_Table.png)

The Easy Ensemble AdaBoost Classifer achieved the best results, with an accuracy score of 92.6%. The other ensemble classifier, Balanced Random Forest, was next with a 78.8% accuracy score. Undersampling with ClusterCentroids achieved the worst results at 51.8%. The two oversampling algorithms, Naïve Random and SMOTE, were both in the middle of the range at a little over 65%, while SMOTEEENN faired slightly worse at just under 64%.

Here is a comparision of the confusion matrices for each of the models:

![Confusion_Matrices.png](Resources/Confusion_Matrices.png)

• TP: True Positive

• FN: False Negative

• FP: False Positive

• TN: True Negative

The data from the confusion matrices show that the two ensemble classifiers produced the smallest number of false diagnoses, with Easy Ensemble AdaBoost classifier producing 953 false positives and only 8 false negatives, for 961 false diagnoses overall. In contrast, the undersampling algorithm producted 9,266 false diagnoses overall, with 9,229 being false negatives.

Here is a comparision of the average metrics from each of the imbalanced classification reports for each of the six models:

![Average_Metrics.png](Resources/Average_Metrics.png)

## Summary of the results

The average precision score for all models was 99%. This was because the number of high-risk credit applications, relative to the number of low-risk credit applications, was small. The significant differences between the models appeared in the other metrics.  

The two ensemble classifiers achieved the best results in the majority of other metrics, including recall, specificity, F1, geometric mean, and index balanced accuracy (ipa). The metrics show that the undersampling model achieved the worst results among the six models. The Naïve Random, SMOTE, and SMOTEENN models achieved results among these metrics that were in the middle between the ensemble classifers and the undersampling model.

## Recommendation of which model to use

The Easy Ensemble AdaBoost Classifier achieved the best results overall. It had the highest balanced accuracy score and presented the best results in its confusion matrix and imbalanced classification report. 

Based on these results, we recommend using the <b>Easy Ensemble AdaBoost Classifier</b> model.
