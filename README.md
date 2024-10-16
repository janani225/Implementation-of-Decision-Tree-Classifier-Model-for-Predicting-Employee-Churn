# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.

2.Upload and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program and Output:
#### Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
#### Developed by:JANANI.V.S
#### RegisterNumber:212222230050
```

import pandas as pd
from sklearn.preprocessing import LabelEncoder
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
from sklearn.tree import DecisionTreeClassifier 
data = pd.read_csv("/content/Employee (1).csv")
data.head()
```
![image](https://github.com/user-attachments/assets/38d7dedf-2e97-433f-a8a0-da81592ad2cb)
```
data.info()
```
![image](https://github.com/user-attachments/assets/75bb0002-1a49-405a-b090-6bc3a6f91810)
```
data.isnull().sum()
```
![image](https://github.com/user-attachments/assets/e91c22a4-88ce-4b9a-a122-ce7afa3e042f)

```
data["left"].value_counts()
```
![image](https://github.com/user-attachments/assets/a8c840a5-d1fe-40f2-8d40-f37c83468081)
```
le = LabelEncoder()
data["salary"] = le.fit_transform(data["salary"])
data.head()
```
![image](https://github.com/user-attachments/assets/8c478d9f-17e6-4130-be05-2e8bf8c2412f)
```
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","promotion_last_5years","salary"]]
x.head()
```
![image](https://github.com/user-attachments/assets/b714f08a-df1e-4271-981b-3ba385d0e8c7)
```
y_pred=dt.predict(x_test)
y_pred
```
![image](https://github.com/user-attachments/assets/e5df3875-96db-46f2-9a62-c72306367fab)

```
accuracy= accuracy_score(y_test,y_pred)
accuracy
```
![image](https://github.com/user-attachments/assets/7d92b35b-a1db-4ef2-80e9-4c2418996da4)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
