# Credit Risk Analysis

CWRU Data Analytics Module Eighteen Challenge


## Overview of Project

The project involved using unsupervised machine learning models with a relatively small crypto currency dataset of ~1100 rows containing information regarding coin name, algorithm used, trading status, proof type, total coines mined and total coin supply. 
  

## Analysis 

The Challenge focused upon pre-processing the data to focus upon the algorithms used for those actively being used for mining, using PCA to identify components upon which to model using K-Means, and then visualizing the results. 


Four LogisticRegression models:  

* after resampling using RandomOverSampler

* after resampling using SMOTE

* after resampling using ClusterCentroids

* after over/under resampling using SMOTEEN 

Two ensemble classifier models:

* using BalancedRandomForestClassifier

* using EasyEnsembleClassifier


### Summary

The ensemble models generally perform better than logistic Regression, with boosting producing better results than bagging.   This is likely due to the underlying data distribution and variance where multiple iterations outperform single iteration modeling.  The Logistic Regression models range in balanced accuracy from .51 to .65 whereas the Ensemble models range from .78 to .92.  I did, however, notice that my results are somewhat different from those in the sample file - which may be due to how I used getdummies(), but our TA indicated the basic results were in line with expectations.  

### Visualzations  


**Elbow curve**

![img](https://github.com/fhsal/Cryptocurrencies/blob/main/images/elbowCurve.png)

**Principle Components Scatter, 2D**

![img](https://github.com/fhsal/Cryptocurrencies/blob/main/images/2dScatter1.png)


**Principle Components Scatter, 3D**  

![img](https://github.com/fhsal/Cryptocurrencies/blob/main/images/3dScatter.png)

**HVplot Table**  

![img](https://github.com/fhsal/Cryptocurrencies/blob/main/images/HVplotTable.png)


**Coins Mined Coins Supply Scatter**

![img](https://github.com/fhsal/Cryptocurrencies/blob/main/images/coinsMinedCoinsSupplyScatter.png)
