# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:

### Step 1
Import pandas from library

### Step 2
import linear_model from sklearn

### Step 3
Read the csv file usingpandas library

### Step 4
Enter the parameters of the linear function.

### Step 5
Print the parameters of the linear function.

## Program:

```
Developed by: S Kantha Sishanth
Register number: 22007660

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
```

## Output:

!['Multivariate'](https://github.com/Skanthasishanth/Multivariate-Linear-Regression/blob/master/imgmul.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
