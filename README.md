# Credit Risk Analyis

## Purpose
This analysis uses 6 different supervised machine learning algorithms to asses credit risk and compares the relative efficacy of the various methods. 
In this analysis the following methods are used
1. Naive Random Oversampling
2. SMOTE Oversampling
3. Cluster Centroids algorithm undersampling
4. SMOTEENN combination sampling
5. Balanced Random Forest Classifer
6. Easy Ensemble AdaBoost Classifier

## Results
The balanced accuracy Scores for each model are as follows

- **Naive Random Oversampling**
    
    Accuracy: .578

    Avg Precision: .99

    High-Risk Precision: .01

    Recall: .58

---
- **SMOTE Oversampling**          
    
    Accuracy: .536

    Avg Precision: .99

    High-Risk Precision: .01

    Recall: .60

---
- **Cluster Centroids**
    
    Accuracy: .501

    Avg Precision: .99

    High-Risk Precision: .01

    Recall: .61

---            
- **SMOTEENN**                      
    
    Accuracy: .674

    Avg Precision: .99

    High-Risk Precision: .01

    Recall: .57

---
- **Balanced Random Forest**
    
    Accuracy: .797

    Avg Precision: .99

    High-Risk Precision: .04

    Recall: .91

---        
- **Ensemble AdaBoost**
    
    Accuracy: .921

    Avg Precision: .99

    High-Risk Precision: .08

    Recall: .94

---

## Summary

All of the models used had a very high average precision. However, only the Balanced Random Forest Classifier and the AdaBoost Classifier had a precision higher than .01 for the high risk credit category, with Ada boost having double that of Balanced Random Forest Classifier at .08. 

The first three methods of Oversampling, SMOTE oversampling, and centroid cluster undersampling had a similar accuracy of around .5. 

The SMOTEENN algorithm had a better accuracy of .674. But the tree methods had by far the best accuracy with the AdaBoost being the clear highest performing model at .921 accuracy. 

I would reccomend using the AdaBoost algorithm because of its high accuracy, and its siginificantly better precision with respect to identifiying high risk loans.