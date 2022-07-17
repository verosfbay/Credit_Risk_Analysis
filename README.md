# Credit Risk Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I’ll need to employ different techniques to train and evaluate models with unbalanced classes. I will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, I’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

### Naive Random Oversampling
* The balanced accuracy score is about 65% (65.47)
<img width="453" alt="Screen Shot 2022-07-17 at 3 56 36 PM" src="https://user-images.githubusercontent.com/95447175/179428108-41332c64-6750-4ac9-9dbf-0b9732f761d7.png">

* The high risk precision rate is 1% with the recall at 64%, the low risk precision rate is 100% with a recall at 69% 
<img width="687" alt="Screen Shot 2022-07-17 at 1 14 03 PM" src="https://user-images.githubusercontent.com/95447175/179423274-6a872a11-9431-4c3b-972c-2448347b3e11.png">

### SMOTE Oversampling 
* The balanced accuracy score is about 66% (66.20) 
<img width="393" alt="Screen Shot 2022-07-17 at 3 56 49 PM" src="https://user-images.githubusercontent.com/95447175/179428117-88e18e32-a23b-4dab-b436-d3742e167a66.png">

* The high risk precision rate is 1% with the recall at 64%, the low risk precision rate is 100% with a recall at 69% 
<img width="665" alt="Screen Shot 2022-07-17 at 1 15 21 PM" src="https://user-images.githubusercontent.com/95447175/179423326-d72058e2-4868-40e3-97c3-c6accc6fe232.png">

### Undersampling
* The balanced accuracy score is about 54% (54.42) 
<img width="432" alt="Screen Shot 2022-07-17 at 3 57 19 PM" src="https://user-images.githubusercontent.com/95447175/179428134-ed8eb381-080d-44af-970e-7dcc59468a61.png">

* The high risk precision rate is 1% with the recall at 69%, the low risk precision rate is 100% with a recall at 40% 
<img width="752" alt="Screen Shot 2022-07-17 at 3 45 02 PM" src="https://user-images.githubusercontent.com/95447175/179427756-4871c57a-65c4-4749-ae1a-f0e48943ed0b.png">

### SMOTEENN Combination Sampling
* The balanced accuracy score is about 65% (64.73)
<img width="471" alt="Screen Shot 2022-07-17 at 3 57 38 PM" src="https://user-images.githubusercontent.com/95447175/179428142-ae3cb8e9-f962-4ff7-a95e-be23387e44dc.png">

* The high risk precision rate is 1% with the recall at 72%, the low risk precision rate is 100% with a recall at 57% 
<img width="767" alt="Screen Shot 2022-07-17 at 3 52 34 PM" src="https://user-images.githubusercontent.com/95447175/179428012-b8e56fcc-13f3-4f29-8389-a5760fc2500b.png">

### BalancedRandomForestClassifier 
* The balanced accuracy score is about 68% (68.30)
<img width="384" alt="Screen Shot 2022-07-17 at 4 03 43 PM" src="https://user-images.githubusercontent.com/95447175/179428316-7135a5af-61e2-4cb9-8033-a2e2b6ecd9b3.png">

* The high risk precision rate is 88% with the recall at 37%, the low risk precision rate is 100% with a recall at 100% 
<img width="699" alt="Screen Shot 2022-07-17 at 4 04 17 PM" src="https://user-images.githubusercontent.com/95447175/179428326-01b3234c-13d8-4a50-b7c8-2ef7bbf4226e.png">

### EasyEnsembleClassifier model
* The balanced accuracy score is about 65% (64.73)


* The high risk precision rate is 1% with the recall at 72%, the low risk precision rate is 100% with a recall at 57% 



## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
