# Data Science Demand Prediction: Project Overview
---
* Model the demand for shared bikes with the available independednt variables
* model Evaluation using R-squared score on the test set
```python
from sklearn.metrics import r2_score
r2_score(y_test,y_pred)
```
* Built multi linear regression model for the prediction of demand

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



