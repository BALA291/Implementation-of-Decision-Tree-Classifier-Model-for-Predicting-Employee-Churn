# EX-06 Implementation of Decision Tree Classifier Model for Predicting Employee Churn
### AIM:
To write a program to implement the Decision Tree Classifier 
Model for Predicting Employee Churn.
### Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook
### Algorithm
1.Import the required libraries.

2.Upload and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5.Find the accuracy of the model and predict the required values by importing the required module from sklearn. 
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: BALAMURUGAN B
RegisterNumber: 212222230016
import pandas as pd
data=pd.read_csv('Employee.csv')
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x = data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion = "entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
 ### DATASET
![head](https://github.com/BALA291/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/120717501/7cfb5638-2b89-4f54-b6a0-caf463f8e134)

### INFO
![info](https://github.com/BALA291/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/120717501/9188ec73-9085-4597-a24a-d4776efeb09d)

### LABEL ENCODING FOR STRING VALUES
![label](https://github.com/BALA291/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/120717501/19fb9ce4-d585-44f7-9282-7a356a7e640c)

### ACCURACY
![accuracy](https://github.com/BALA291/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/120717501/1a387815-1a5b-4f98-ada5-5102e53d090a)

### PREDICTION
![prediction](https://github.com/BALA291/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/120717501/7d308a3f-5dc2-4f86-872c-8ac634345cf2)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
