# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of x and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg,and the volume is 1300cm cube.
### Step6
Print the predicted output.

## Program:
```
#To write a python program to implement multivariate linear regression and predict the output.
#Developed by: paida ram sai
#Ref.No: 23007931

import pandas as pd
from sklearn import linear_model
import matplotlib.pyplot as plt

df=pd.read_csv("cars.csv")

x=df[['Weight', 'Volume']]
y=df['CO2']

regr=linear_model.LinearRegression()
regr.fit(x,y)

#coefficients and intercept of model
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2= regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![image](https://github.com/ramsai22/Multivariate-Linear-Regression/assets/150319855/a494217f-464e-404a-95d1-b863e7c77a10)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
