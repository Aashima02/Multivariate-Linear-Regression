# Implementation of Multivariate Linear Regression
## AIM:
To write a python program to implement multivariate linear regression and predict the output.

## EQUIPMENT'S REQUIRED:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
### Step1: 
Import pandas as pd.
### Step2: 
Read the csv file.
### Step3: 
Get the value of X and y variables.
### Step4: 
Create the linear regression model and fit.
### Step5: 
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.
### Step6: 
Print the predicted output.

## PROGRAM:
```
To write a python program to implement multivariate linear regression.
Developed by: Aashima Nazreen Sayeed S
Register Number: 21500368

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
x = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume is",predictedCO2)

```
## OUTPUT:
![output](./output.png)



## RESULT:
Thus the multivariate linear regression is implemented and predicted the output using python program.