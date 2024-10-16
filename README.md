# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1.Import Libraries: Load necessary libraries (Pandas, Scikit-learn).
2.Load Data: Read the employee data from a CSV file.
3.Explore Data: Display dataset information and check for missing values.
4.Preprocess Data: Encode categorical variables and define features (X) and target (y).
5.Split Data: Divide the data into training (80%) and testing (20%) sets.
6.Train Model: Initialize and fit a Decision Tree Classifier on the training data.
7.Make Predictions: Predict employee churn on the test set.
8.Evaluate Model: Calculate and display the model's accuracy.
```

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SRIKAAVYAA T
RegisterNumber:  212223230214
*/
```

```
import pandas as pd
data=pd.read_csv("Employee.csv")

data.head()

```
## Output:

![Screenshot 2024-10-16 155300](https://github.com/user-attachments/assets/35b4fec7-9caa-4661-8942-67ebb368e278)


```
data.info()
```


![Screenshot 2024-10-16 155343](https://github.com/user-attachments/assets/c267dd06-7096-4603-931e-b06a2b7d0144)


```
data.isnull().sum()

```

![Screenshot 2024-10-16 155419](https://github.com/user-attachments/assets/8b2e79e3-59da-48fa-8427-04a663dcb49f)


```
data["left"].value_counts()
```

![Screenshot 2024-10-16 155557](https://github.com/user-attachments/assets/92cbb3a2-eb9b-4715-94c0-af6daf1540b5)


```
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
```

![Screenshot 2024-10-16 155707](https://github.com/user-attachments/assets/01fbe9c1-cfae-4c0f-9f19-dda4cb1a4e01)
![Screenshot 2024-10-16 155719](https://github.com/user-attachments/assets/51f71b7d-7107-4cb4-b8cf-442bc9eccd95)

## OUTPUT

![Screenshot 2024-10-16 155728](https://github.com/user-attachments/assets/2f287913-7416-4c0e-bbf3-577f17d76e70)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
