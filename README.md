# Project2

---
### Question: What are the best features to predict heart disease?
The following models are trying to predict heart disease amongst people based on their biomedical data. That data includes information on the patient's age, resting blood pressure, cholesterol, fasting blood sugar, their max heart rate, and oldpeak. What was found in the data is that the 3 features with greatest corelation, positive or negative, with heart diseae are age, max heart rate, and oldpeak. 

---
### First Insight
Max heart rate delines as people age: as people age their is downward trend where their max heart rate declines.

![image](https://user-images.githubusercontent.com/49537432/222751037-4ba26c87-3ac7-447d-bc8c-eff93eacfdfa.png)

---
### Second Insight
Oldpeak increase as people get older: No one under 50 had an oldpeak over 4 while and oldpeak of 6 was one of the common values for those over 50. Unlike with max heart rate a lower number is better in this circumstance. 

![image](https://user-images.githubusercontent.com/49537432/222756230-d9c572d5-aff5-442c-928b-3105dd850b63.png)

---
### Model Analysis

The model I would recomend for indentifying heart disease in people is a logisitic regression model. It had the highest recall on the testing data of 78%. Recall is the most important metric in this data because a false negative is the most dangerous scenario. A false negative in this instance would mean that a person is falsely identified of being free of heart disease when they in face have it. A false negative would therefore lead a patient to not recieve the treatment they need and may lead to serious illness or even death. 

              precision    recall  f1-score   support

           0       0.69      0.67      0.68        98
           1       0.76      0.78      0.77       132

    accuracy                           0.73       230
   macro avg       0.73      0.73      0.73       230
weighted avg       0.73      0.73      0.73       230
