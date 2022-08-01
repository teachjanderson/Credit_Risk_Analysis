# Credit Risk Analysis

## Overview

Credit risk involves identifying good loans compared to risky loans; however, there is an unbalanced classification problem as the good loans outnumber the riskier ones. By employing different techniques to train and evaluate models with unbalanced classes, using the ['Imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn) and ['Scikit-Learn'](https://github.com/scikit-learn/scikit-learn) libraries, we can evaluate the models by resampling. 

The datasets from LendingClub, a peer-to-peer lending services, provided data to oversample using 'RandomOverSampler' and 'Smote' algorithms and the 'ClusterCentroid' algorithm to undersample. To provide a combinatorial approach of over- and undersampling, the analysis used the 'SMOTEEN' algorithm. Finally, machine learning models including 'BalancedRandomForestClassifier' and 'EasyEnsembleClassifier' were employed to reduce bias and predict credit risk. The following summary outlines the results of this analysis. 

This analysis also included the [Numpy](https://numpy.org/), [Pathlib](https://docs.python.org/3/library/pathlib.html), and [Pandas](https://pandas.pydata.org/) libraries. 

## Results

This analysis employed Machine Learning by using Python libraries referenced above. All together, six machine learning models evaluated the credit risk. In each case, the 'loan status' of each individual was the targeted factor. 

# 1. Naive Random Oversampling

* Accuracy Score: 67%
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />

# 2. SMOTE Oversampling

* Accuracy Score: 66%
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />

# 3. Cluster Centroids Undersampling

* Accuracy Score:
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />

# 4. Combination Sampling

* Accuracy Score:
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />

# 5. Balanced Random Forest Classifier

* Accuracy Score:
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />

# 6. Easy Ensemble Classifier

* Accuracy Score:
* Precision High Risk:
* Precision Low Risk:
* Recall High Risk:
* Recall Low Risk: 

Classification Report 

<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />



There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.


<p align="center"><img src="https://github.com/teachjanderson/Amazon_Vine_Analysis/blob/main/Project_Images/VineTotal3.png" width="600" />


# Summary: 

There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


