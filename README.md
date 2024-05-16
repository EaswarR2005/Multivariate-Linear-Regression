# Implementation of Multivariate Linear Regression:
## Aim:
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
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
## Program:
```
NAME: EASWAR R
REGISTER NUMBER: 212223230053

import pandas as pd
from sklearn import linear_model
data=pd.read_csv('car.csv')
x=data[['Weight','Volume']]
y=data['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficient:",regression.coef_)
print("Intercept:",regression.intercept_)
predictCO2=regression.predict([[3300,1300]])
print("CO2 required is",predictCO2)
```
## Output:
![image](https://github.com/EaswarR2005/Multivariate-Linear-Regression/assets/146931525/cae5aeeb-5c64-47aa-97c5-9271139b0b0c)


## Result:
Thus the multivariate linear regression is implemented and predicted the output using python program.
