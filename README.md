# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas and necessary packages to process the dataset.
<br>

### Step2
By Accessing the Packages, use the functions to read input and store as csv file.
<br>

### Step3
Feeding x, y and regr values.
<br>

### Step4
Forming line of best fit and finding predicted values and printing the coefficients,intercepts and predicted values.
<br>

### Step5
Displaying output and Result.
<br>

## Program:
```
#Developed By: Harish Bakavadh J
#Register Number: 26007865 
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)






```
## Output:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e5869444-2408-47de-818a-36a128601601" />


### Insert your output
Coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO2 for the corresponding weight and volume: [114.75968007]

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
