# Data Science Demand Prediction: Project Overview
---
- A bike sharing company wants to understand the factors on which the demand for the bikes depend
- Which variables are significant in predicting the demand for shared bikes
- how well those variables describe the bike demands
* model Evaluation using R-squared score on the test set
```python
from sklearn.metrics import r2_score
r2_score(y_test,y_pred)
```
* Used linear regression model for the prediction of demand

## Code and Resources Used
---
**Python Version:** 3.7 <br>
**Packages:** pandas, numpy, sklearn, statsmodel, matplotlib, seaborn

## Data Preparation and Cleaning
---
* `season` column has 1,2,3,4 representing **spring, summer, fall, winter** which is continous and hence changed to categorical as to avoid class imbalance
* Data has a lot of columns which needs to be categorical but represented as continous hence performing data manipulation to convert them to categorical variables

## EDA
---
I Looked at the distribution of data with subplots and heatmaps to find the max correlation between features
![linear reg git hub](https://user-images.githubusercontent.com/69252134/130642090-fdb29c03-295e-49f1-a95c-d26fa153974b.png)
* Found that `cnt` is highly correlated with `temp` surely we know that this is the most important feature in model building on primary analysis

## Model Building
---
First I transformed the categorical variables into dummy variables. I also split the data into train and test sets with test size of 30% Scaled the data using minmax scalar

I tried **Linear regression** model with stats  & sklearn packages,in identifying most important feature and dropped variables with **high p values with significance level of 0.05 and VIF grater than 5**

I chose **R2 score** to evaluate the model performance

## Model Performance
---
MOdel has performed significantly well on linear regression with

* **r2_score** = **0.82**



