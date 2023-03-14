# Project2

Joseph Cobbs
josephecobbs@gmail.com


---
###

Each row in this data set represents one patient and their individual health data related to heart disease. The data in

Age 
Resting Blood Pressure 
Cholesterol 
Fasting Blood Sugar 
Max Heart Rate
Oldpeak
Heart Disease 
Sex
Chest Pain Type
Resting ECG
Exercise Angina
ST Slope


---
### Question: What are the best features to predict heart disease?
The following models are trying to predict heart disease amongst people based on their biomedical data. That data includes information on the patient's age, resting blood pressure, cholesterol, fasting blood sugar, their max heart rate, and oldpeak. What was found in the data is that the 3 features with greatest corelation, positive or negative, with heart diseae are age, max heart rate, and oldpeak. 

---
### First Insight
Max heart rate delines as people age: as people age their is downward trend where their max heart rate declines.

![image](https://user-images.githubusercontent.com/49537432/225137283-df658c7e-3b51-4145-b749-6f0af2de7d27.png)

---
### Second Insight
Oldpeak increase as people get older: No one under 50 had an oldpeak over 4 while and oldpeak of 6 was one of the common values for those over 50. Unlike with max heart rate a lower number is better in this circumstance. 

![image](https://user-images.githubusercontent.com/49537432/222756230-d9c572d5-aff5-442c-928b-3105dd850b63.png)

---
### Model Analysis

The model I would recomend for indentifying heart disease in people is a logisitic regression model. It had the highest recall on the testing data of 78%. Recall is the most important metric in this data because a false negative is the most dangerous scenario. A false negative in this instance would mean that a person is falsely identified of being free of heart disease when they in face have it. A false negative would therefore lead a patient to not recieve the treatment they need and may lead to serious illness or even death. 

       precision    recall  f1-score   support

           0       0.79      0.86      0.82        98
           1       0.89      0.83      0.85       132

    accuracy                           0.84       230
   macro avg       0.84      0.84      0.84       230
weighted avg       0.84      0.84      0.84       230


The model would preform adequately to identify potential heart disease, with a recall score of 89% it will catch roughly 9/10 false negatives ensuring the cast majority of patients will know that they have heart disease in the instance where they do have it. However, with such a serious condition being underconsideration more data is needed to improve model outcomes and thus patient outcomes. 

---

### Recommendations 
---
1. With such a small sample size of less that a 1000 it is challenging to make a predictive model with high accuracy. Therefore, more data is needed. More data would also increase variety in the data and lead to including more people of different health backgrounds creating a more all encompassing model. 
2. To idenfity heart disease in patients look primarily at their age, max heart rate, and oldpeak. These were the only features with a medium correlation with heart disease our target. 
