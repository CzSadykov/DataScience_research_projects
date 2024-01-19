# Predicting an optimal oil well location

**Problem situation**: On assignment for a fictitious mining company we help to decide where to drill a new oil well.

**Goal**: to determine the most profitable region for the development of oil wells.

**Tasks**:

1. Build a machine learning model that will help determine the region where mining will bring the most profit.
2. Analyze possible profits and risks using the *Bootstrap* technique

**Data**:

The data is taken from the exploration of three regions, each dataset contains 100,000 observations.
List of variables:

* ```id``` — unique identifier of the well;
* ```f0, f1, f2``` - well characteristics;
* **```product```** — volume of reserves in the well (in thousands of barrels). That's our target variable.

## Conclusions

Based on the results of the analysis, we  recommend region 2 for the development. Reasons for that are:

* Probability of losses: **1%**;
* Projected average profit:**477,052,540** rubles;
* With a 95% probability, the average profit will be in the range from **74,463,435** to **888,676,356** rubles.

The model used is linear regression. Moreover, for the second region, the model turned out to be of the highest quality. Apparently, due to the specifics of the input data. Our final metrics:

* RMSE: 0.89
* R^2: 0.99962
* MAE: 0.72
