# Credit Risk Analysis

## Overview of Project
For this challenge, I built, trained, and analyzed different models that used unbalanced classes in order to create a model that most accurately assesses credit card risk.

## Results

### Oversampling
#### RandomOverSampler
![Screen Shot 2022-07-24 at 10 47 41 PM](https://user-images.githubusercontent.com/101145419/180700728-6301286a-1525-47fa-8811-d186694cdb3d.png)
- the balanced accuracy score was 58%
- high risk
  - precision rate: 1%
  - recall rate: 74%
- low risk
  - precision rate: 100%
  - recall rate: 55%

![Screen Shot 2022-07-24 at 10 47 54 PM](https://user-images.githubusercontent.com/101145419/180700738-556c1873-235e-46e3-a7b8-7c767f5737c2.png)

#### SMOTE
![Screen Shot 2022-07-24 at 10 48 04 PM](https://user-images.githubusercontent.com/101145419/180700743-c74f9433-78b9-4c42-ac34-c464f1577ae0.png)
- the balanced accuracy score was 64%
- high risk
  - precision rate: 1%
  - recall rate: 54%
- low risk
  - precision rate: 100%
  - recall rate: 74%
![Screen Shot 2022-07-24 at 10 48 10 PM](https://user-images.githubusercontent.com/101145419/180700767-9cfb4623-6e60-4f89-81ad-974f5b3de6d4.png)


### Undersampling
#### ClusterCentroids
![Screen Shot 2022-07-24 at 10 49 55 PM](https://user-images.githubusercontent.com/101145419/180700832-c4e898b6-7739-4596-b51b-555225ccc0e5.png)
- the balanced accuracy score was 54%
- high risk
  - precision rate: 1%
  - recall rate: 67%
- low risk
  - precision rate: 100%
  - recall rate: 42%
![Screen Shot 2022-07-24 at 10 50 00 PM](https://user-images.githubusercontent.com/101145419/180700838-731bb52d-bef5-41ac-b1f0-e086a63ac17f.png)


### Combination Approach
#### SMOTEENN
![Screen Shot 2022-07-24 at 10 50 33 PM](https://user-images.githubusercontent.com/101145419/180700891-5c91e7ff-450b-4cef-b41c-f51c2e5076fe.png)
- the balanced accuracy score was 53%
- high risk
  - precision rate: 1%
  - recall rate: 53%
- low risk
  - precision rate: 99%
  - recall rate: 53%
![Screen Shot 2022-07-24 at 10 50 38 PM](https://user-images.githubusercontent.com/101145419/180700903-2b2a80f5-56e5-4680-8b5d-438427f0c5dd.png)

### Newer Models
#### BalancedRandomForestClassifier
![Screen Shot 2022-07-24 at 11 49 37 PM](https://user-images.githubusercontent.com/101145419/180707498-4c89a3f2-5537-4a3a-90c5-c3b26378fea0.png)
- the balanced accuracy score was 53%
- high risk
  - precision rate: 1%
  - recall rate: 53%
- low risk
  - precision rate: 99%
  - recall rate: 53%
![Screen Shot 2022-07-24 at 11 49 41 PM](https://user-images.githubusercontent.com/101145419/180707514-6e643b05-4a14-465d-ba4a-d63539948a1f.png)

#### EasyEnsembleClassifier
![Screen Shot 2022-07-24 at 11 49 47 PM](https://user-images.githubusercontent.com/101145419/180707526-87e6d8e2-f2a4-4ada-a1b1-cc570cb5aa20.png)
- the balanced accuracy score was 53%
- high risk
  - precision rate: 1%
  - recall rate: 53%
- low risk
  - precision rate: 99%
  - recall rate: 53%
![Screen Shot 2022-07-24 at 11 49 52 PM](https://user-images.githubusercontent.com/101145419/180707536-46d4b6bf-8782-4acb-b2c2-0d817c311d4d.png)

## Summary
Overall, majority of the models were not able to produce desirable balanced accuracy scores. However, both of the Newer Models performed well. Although both had respectable balanced accuracy scores, only the EasyEnsembleClassifier exceeded 90%. Based on this information, I would only recommend using the EasyEnsembleClassifier. 
