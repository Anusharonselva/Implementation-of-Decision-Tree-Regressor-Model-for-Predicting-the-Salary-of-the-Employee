# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the libraries and read the data frame using pandas.
2. Calculate the null values present in the dataset and apply label encoder.
3. Determine test and training data set and apply decison tree regression in dataset.
4. calculate Mean square error,data prediction and r2.


## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: S.ANUSHARON
RegisterNumber:  212222240010

import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data[["Salary"]]
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])

*/
```

## Output:

data.head()

![Screenshot (301)](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/1f9b2fb5-7e2d-476d-868e-b7efde32b345)

data.info()

![Screenshot (301) 1](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/7d74f543-831d-4f0e-97da-db4d1682fda5)

isnull() and sum()

![Screenshot (302)](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/b43672a4-160c-4de1-91b2-72bbddd6682e)

data.head() for salary

![Screenshot (302) 1](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/9b9ef48c-5644-4d6a-b410-ff5b9973b9ff)

MSE value

![Screenshot (302) 2](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/0a46dada-e416-4417-a0c4-a6a75dacda0d)

r2 value

![Screenshot (302) 3](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/d94c9931-3525-4ad9-b343-21c688c44162)

data prediction

![Screenshot (303)](https://github.com/Anusharonselva/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119405600/f3361206-9aff-44e2-bfdf-5df3662d3df7)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
