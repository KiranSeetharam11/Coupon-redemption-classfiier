
# Coupon Redemption Classifier

Customers are more likely to purchase in the store if there is a discount that looks profitable to them. Coupons are best used to ensure business happens in the store with a small discount in the margin. It is important to know who is the best potential users of the coupon to maximise sales.

# Project Overview

This project develops a RandomForestClassifier Model that classifies the customers by using features from multiple files which are linked by primary keys

It uses 7 datasets - each with different data that is put together to form feature columns







## Data Background
The dataset to train the model is from Kaggle
[DATASET](https://www.kaggle.com/datasets/meghakanojia/predicting-coupon-redemption)

It has 7 tables which are linked by keys which is present in the test.csv




## Run Locally

To run this project locally, ensure you have the following libraries installed:

```bash
  pip install pandas
  pip install numpy
  pip install scikit-learn
```
    
## Structure of the project


### Data Cleaning
- Check and handle Null values, the dataset had few NaN values which was handled using replace function

### Feature Engineering
- Use one-hot Encoding by using pandas.dummies()

### Merging Databases
- All important feature columsn were retained and others were deleted
- Based on common columns(primary keys), the dataset was merged using pandas.merge
- Due to high amount of data, sample data was taken as a part of the whole data to avoid storage isseus.

### Model Training
- A RandomForestClassifier Model was created and trained with the above data.


### Performance
-  The cross validation score obtained was 0.9683 


## ER Diagram

![ER Diagram](https://github.com/KiranSeetharam11/Cheque-Details-Recognition/blob/main/Cheque%20ER.png)

