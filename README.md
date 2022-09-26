# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1


### Step2


### Step3


### Step4


### Step5


## Program:
```python
import pandas as pd
from sklearn import linear_model

data=pd.read_csv("cars.csv")

X=data[['Weight','Volume']]
Y=data[['CO2']]

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding Weight and Volume: ",predictCO2)


```
## Output:

![output](./carsout.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
