# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas.
### Step2
Import linear model from sklearn
### Step3
Read the files cars[1].csv
### Step4
Assign the values for a and b as requried.
### Step5
Create the LinearRegression model and predict the output

## Program:
```

#Program for Multivariate Linear Regression
#Developed by: SHYAM S
#Register Number: 23012478

import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars[1].csv')
a=df[["Weight","Volume"]]
b=df[["CO2"]]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))

```
## Output:


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
