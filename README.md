# Predicting a number of taxi orders (time series ML)

**Goal:** Our fictional customer wants to attract more drivers during peak periods.

**Task:** build a model to predict the number of taxi orders for the next hour. As part of this work, we will use **linear regression**, as well as models based on gradient boosting - **Light GBM** and **CatBoost**. Of these, we will choose the best one based on prediction quality metrics and training time.

**Data:** Historical data on taxi orders at airports. Features: number of orders (target feature), date/time.

**Initial requirements:**

* Period for resampling: 1 hour;
* The test sample percentage: 10% of the original data;
* The value of an *RMSE* metric on the test sample should not exceed 48.
  
## Results

**Best Model**

A cost-efficient linear regression trained with cross-validation for 5-block time series in basically zero time.
**Final RMSE:** 34.201. 

Training and testing was carried out on the basis of features extended by 168 time lags (where each lag is 1 hour of observations) and a moving average taken for 24-hour windows.
