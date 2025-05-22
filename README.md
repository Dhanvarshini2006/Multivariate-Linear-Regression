# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import necessary libraries and load the dataset into a DataFrame using pandas.
### Step2
Define the independent variables (Volume, Weight) as x, and the dependent variable (CO2) as y.

### Step3
Initialize a linear regression model and fit it to the data.

### Step4
Output the learned coefficients (slopes) and the intercept (bias term).

### Step5
Use the trained model to predict CO2 emission for a new input (Volume=1300, Weight=1300).

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/car (1) (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression= linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[1300,1300]]))


```
## Output:

![alt text](<WhatsApp Image 2025-05-22 at 14.34.44_4112b6aa.jpg>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.