# Credit Risk Analysis

## Overview

Credit risk involves identifying good loans compared to risky loans; however, there is an unbalanced classification problem as the good loans outnumber the riskier ones. By employing different techniques to train and evaluate models with unbalanced classes, using the ['Imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn) and ['Scikit-Learn'](https://github.com/scikit-learn/scikit-learn) libraries, we can evaluate the models by resampling. 

The datasets from LendingClub, a peer-to-peer lending services, provided data to oversample using 'RandomOverSampler' and 'Smote' algorithms and the 'ClusterCentroid' algorithm to undersample. To provide a combinatorial approach of over- and undersampling, the analysis used the 'SMOTEEN' algorithm. Finally, machine learning models including 'BalancedRandomForestClassifier' and 'EasyEnsembleClassifier' were employed to reduce bias and predict credit risk. The following summary outlines the results of this analysis. 

This analysis also included the [Numpy](https://numpy.org/), [Pathlib](https://docs.python.org/3/library/pathlib.html), and [Pandas](https://pandas.pydata.org/) libraries. 

## Results

This analysis employed Machine Learning by using Python libraries referenced above. All together, six machine learning models evaluated the credit risk. In each case, the 'loan status' of each individual was the targeted factor. 

# 1. Naive Random Oversampling

* Accuracy Score: 67%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 74%
* Recall Low Risk: 61%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Naive.png" width="600" />

# 2. SMOTE Oversampling

* Accuracy Score: 66%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 63%
* Recall Low Risk: 69%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-07-31%20at%2011.09.35%20PM.png" width="600" />

# 3. Cluster Centroids Undersampling

* Accuracy Score: 54%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 69%
* Recall Low Risk: 40%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Cluster.png" width="600" />

# 4. Combination Sampling

* Accuracy Score: 54%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 73%
* Recall Low Risk: 59%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Combo.png" width="600" />

# 5. Balanced Random Forest Classifier

* Accuracy Score: 75%
* Precision High Risk: 3%
* Precision Low Risk: 100%
* Recall High Risk: 62%
* Recall Low Risk: 89%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Forest.png" width="600" />

# 6. Easy Ensemble Classifier

* Accuracy Score: 93%
* Precision High Risk: 9%
* Precision Low Risk: 100%
* Recall High Risk: 92%
* Recall Low Risk: 94%

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Credit_Risk_Analysis/blob/main/Resources/Easy.png" width="600" />

# Explanations

* Accuracy Score: This score measures the likelihood the model identifes predictions correctly. 
* Precision: This score measures the ability to identify samples accurately and accurately determine positives and negatives in the sets. 
* Recall - Sensitivity: This score measures the sensitivity to finding the positives and negatives in the set. In this analysis, it determines the likelihood a high risk is correctly identified and a low risk is correctly identified. 

Each machine learning model above shows these scores along with the classification report. While all models display accuracy scores above 50%, the Balanced Random Forest Classifier (73%) and the Easy Ensemble Classifier (93%) demonstrate accuracy levels far greater than the others. Similarly, both these models have a precision level equal or greater than the others, but their sensitivity scores are much higher than the average of the other models. 


# Summary: 

In recommending a model to determine credit risk, the error should fall on mis-identifying low-risk as high-risk than the other way around. The Easy Ensemble Classifier not only has the highest accuracy (modeling and predicting accurately), but the highest sensitivity for ensuring accurate placement. 

Once caveat in this dataset is a limited number of 'high risk' individuals. The model used 68,470 low risk data points and 347 high risk data points. This represents a comparison of less than 1% high risk in the modeling. As the dataset used in the modeling is of utmost importance as to not overfit a trend, it's important to consider using various datasets to determind the most accuracy. 

