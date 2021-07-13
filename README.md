# Credit_Risk_Analysis

## __Overview:__


This analysis is mainly aimed at eliminating class imbalances when studying data related to credit card risk. The data is resampled using imbalanced-learn and scikit-learn libraries. Different techniques such as RandomOverSampler, SMOTE algorithms and ClusterCentroids algorithms are applied to oversample and undersample the data and to train and evaluate models with unbalanced classes.


## __Results:__

The results from the various machine learning models are listed below:

- ### Naive Random Oversampling:
    Balanced Accuracy score: 0.618

    Precision and recall scores:

    ![NaiveRandomOversampling](Images/NaiveRandomOversampling.png)

- ### SMOTE Oversampling:
    Balanced Accuracy score: 0.628

    Precision and recall scores:
    ![SMOTEOversampling](Images/SMOTEOversampling.png)

- ### Cluster Centroids Undersampling:
    Balanced Accuracy score: 0.505

    Precision and recall scores:
    ![Cluster_Centroids](Images/Cluster_Centroids.png)

- ### SMOTEENN Under and over sampling:
    Balanced Accuracy score: 0.640

    Precision and recall scores:
    ![SMOTEENN](Images/SMOTEENN.png)

- ### Balanced Random Forest Classifier:
    Balanced Accuracy score: 0.788

    Precision and recall scores:
     ![BalancedRandomForest](Images/BalancedRandomForest.png)

- ### Easy Ensemble AdaBoost Classifier
    Balanced Accuracy score: 0.929

    Precision and recall scores:
    ![EasyEnsembleAdaBoost](Images/EasyEnsembleAdaBoost.png)


## __Summary:__

From the results above it can be seen that the accuracy score is least for the Cluster centroids model at 0.505 and is highest at 0.929 for the Easy Ensemble Clasifier. Therefore as far as accuracy is concerned, the Easy Ensemble Classifier model shows the least difference between predicted and actual values.

The precision score is the highest in the Easy Ensemble Adaboost Classifier model for high risk category of loans. For low risk category, all models have a precision of 1.00. 
This means that there are no false positives for low risk loans and the model predicts low risk loans correctly 100% of the time. Whereas for high risk loans, the numbers indicate that the number of false positives is very high. 

A higher recall score means that the percentage of correctly predicted positives is higher and the number of false negatives is lower. The Easy Rnsemble AdaBoost classifier module has a high recall score for both high risk and low risk categories.

Among all models, the Easy Ensemble Adaboost Classifier model has the highest accuracy score, a comparatively higher precision score and the highest recall score. A high recall score is important especially while predicting high risk loans. Therefore the Easy Ensemble Classifier model is recommended over other models, but steps need to be taken to improve its precision.