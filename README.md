# Module 12 Report Template

## Overview of the Analysis

Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. Using a dataset of historical lending activity from a peer-to-peer lending services company, purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.

Various techniques were utilized in this analysis to train and assess models with imbalanced classes. The original dataset was examined using value_counts and subsequently resampled to enhance the model's prediction accuracy. The imbalanced-learn library was employed to define a logistic regression model, comparing two versions of the dataset: the original dataset and the resampled dataset generated using the RandomOverSampler module. The analysis involved using the LogisticRegression classifier and the resampled data to fit the model and make predictions. The RandomOverSampler module was used to resample the data in both cases. The count of target classes was analyzed, and a logistic regression classifier was trained, followed by the calculation of the balanced accuracy score, generation of a confusion matrix, and production of a classification report.

## Results

* Machine Learning Model 1:
  *  Logistic Regression Model with the Original Data
        * Accuracy: 95.20%  
        * Precision: 85% 
        * Recall: 91%
<br></br>
* Machine Learning Model 2:
  * Logistic Regression Model with Resampled Training Data
    * Accuracy: 99%  
    * Precision: 84% 
    * Recall: 99%


## Summary

By resampling the lending data and employing the Logistic Regression model, higher accuracy was achieved compared to the original data set. This is due to the resampled training data producing higher recall and accuracy scores. Identifying High-risk loans ("1") is more crucial than Healthy Loans ("0"). The recall score for High-risk loans when utilizing the Logistic Regression model on the original data set was 91%, whereas it increased to 99% with the resampled data. Additionally, the accuracy score for High-risk loans using the Logistic Regression model on the original data set was 95%, but it improved to 99% with the resampled data. Consequently, the Logistic Regression Model utilizing Resampled Training Data exhibits superior performance in assessing the creditworthiness of borrowers.
