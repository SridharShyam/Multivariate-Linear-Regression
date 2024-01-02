# Implementation of Multivariate Linear Regression
### NAME: SHYAM S
### REG.NO: 23012478
### DEPT: AIML
## Aim:
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:
Import pandas.
### Step 2:
Import linear model from sklearn.
### Step 3:
Read the files cars[1].csv.
### Step 4:
Assign the values for a and b as requried.
### Step 5:
Create the LinearRegression model and predict the output.
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

![Screenshot 2024-01-02 204513](https://github.com/SridharShyam/Multivariate-Linear-Regression/assets/144871368/d445320a-bfe2-4942-82a1-15dc80157d5a)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
