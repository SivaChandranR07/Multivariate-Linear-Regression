# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1:

Import pandas as pd

### Step2:

Read the csv file.

### Step3:

Get the values of X and Y variable.

### Step4:

Create the linear regression and fit.

### Step5:

Predict CO2 with appropriate values.

### Step6:

Display the predicted value.

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

![output](./cluster.png)
![output](./clusterout.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
