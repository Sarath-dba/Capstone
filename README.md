# 🎓 Student Performance Grade Prediction

## ❓ Problem Statement: 

Provide actionable insights to Schools, teachers and policy makers to plan and design their programs to boost student performance through guidance and mentoring which can result in better academic outcomes.

## 🎯 Model Outcomes or Predictions: 

•	This project uses Machine Learning techniques to analyze student performance based on various features like attendance, study habits, prior grades, and socio-economic factors.

•	The model predicts the future grade of the students and provides opportunities for parents, policy makers, teachers & tutors to proactively involve and contribute to the student’s success.

## 📥 Data Acquisition: 

The dataset is downloaded from Kaggle in CSV format and included as part of documentation. Careful consideration is given to selecting a dataset that encompasses key factors influencing performance through grades. While visualization and correlation analysis highlight major contributors to predictive outcomes, it is important to recognize that other features can indirectly impact these primary contributors.

## 🧑‍💻 Data Preprocessing/Preparation: 

Training a machine learning model needs data to be cleaned, transformed, and structured for better accuracy. 
This step involves handling missing values, encoding categorical variables, scaling numerical features, and selecting relevant features. 
Proper preprocessing ensures the dataset is optimized for model training, improving performance and reducing bias.

•	Handled missing data using Mode based imputation

•	Encoded the categorical features using Ordinal Encoder and One Hot Encoder.

•	Numerical data is scaled using Standard Scaler.

•	The data is split into train and test sets with 80% training size and 20% test size.

## 🧮 Modeling 
The problem is classification problem as we predict the student grade based on available features. Also, we have multiple classes for prediction. We have considered the following models to solve this problem.

a.	Decision Trees
b.	KNN
c.	Random Forests
d.	SVM
e.	XGBoost
f.	Logistic Regression

We then perform GridSearchCV to perform cross validation and hyper parameter tuning to get better evaluation metrics so that the model performs well for unseen data. 

## 📊 Model Evaluation

Based on the above training, testing, validation and tuning of the models, we consider the below evaluation metrics to pick best model for our problem. 

Evaluation metrics for this classification:
a.	Accuracy – How well the model predicts the student grade.
b.	Precision - How well the model predicts the higher-grade students
c.	Recall – How well the model predicts the lower grade students
d.	F1 score – How well the model classifies both higher and lower grade students.
e.	Confusion matrix – Matrix that show case actual and misclassified predictions.

The model with the best accuracy, F1 score, and recall will be selected for these predictions. It is essential to predict student grades accurately and address the performance of lower-performing students without negatively impacting the grades of high-performing students.

•	In this classification problem:
False Positive: Higher-grade students are classified into lower grades, which is acceptable as they can receive guidance.
False Negative: Lower-grade students are classified into higher grades, which is problematic since they might miss needed guidance.

•	We must rank models based on metrics that minimize False Negatives while balancing False Positives and Negatives.
•	XGBoost appears to be the best model for this issue.
•	XGBoost excels in Recall and F1 Score, essential for our imbalanced dataset.
•	Attendance, Hours_Studied, Access_to_Resources, Parental_Involvement, Internet Access seems to be top 5 Important features.
•	From personal experience as a student, the important features given by the model seems obvious in improving better academic performance.

## 💡 Insights

#### •	Takeaways
1.	Attendance at school and study hours are significant factors in achieving good grades.
2.	Access to appropriate resources is important for academic success.
3.	Positive peer influence, parental involvement, and educational background have a beneficial effect on student performance.
4.	There are several indirect factors that can contribute to a student's personal growth, such as physical activity and motivation levels.
   
#### •	Recommendations
##### Schools:
1.	Encourage students to maintain consistent attendance.
2.	Design awareness programs to increase study hours outside of school.
3.	Facilitate student participation in physical and extracurricular activities for personal development.
##### Policy makers:
1.	Provide necessary resources for all students to enhance their studies.
2.	Develop assistance and relief programs to offer internet services to students from low-income families.
##### Teachers & Educators:
1.	Identify students with declining grade predictions compared to previous scores and schedule interactive sessions.
2.	Proactively engage with students and provide guidance to improve their motivation for academic success.

#### •	Future Scope
1.	Information related to social interactions can yield deeper insights.
2.	Features reflecting student interests can enhance understanding and guide them in specific areas.
3.	Plans for college education and career interests can facilitate mentorship and guidance accordingly.

# Project Contributors
This project was developed by Sarath Pericharla as part of Capstone Project under the supervision of Professor Viviana Márquez 👩‍🏫👏🙏
