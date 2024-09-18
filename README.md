# -Afnan-Khaled-Al-Ashwal-202073138-
Diabetes Prediction Project
The Diabetes prediction dataset is a collection of medical and demographic data from patients, along with their diabetes status (positive or negative). The data includes features such as age, gender, body mass index (BMI), hypertension, heart disease, smoking history, HbA1c level, and blood glucose level. This dataset can be used to build machine learning models to predict diabetes in patients based on their medical history and demographic information. This can be useful for healthcare professionals in identifying patients who may be at risk of developing diabetes and in developing personalized treatment plans. Additionally, the dataset can be used by researchers to explore the relationships between various medical and demographic factors and the likelihood of developing diabetes.
3	Dataset Overview
The dataset utilized for this project is the Pima Indians Diabetes Database, which contains 768 instances and 8 attributes. The attributes are as follows:
1.	Pregnancies: Number of times the patient has been pregnant.
2.	Glucose Level: Blood glucose concentration.
3.	Blood Pressure: Diastolic blood pressure (mm Hg).
4.	Skin Thickness: Triceps skin fold thickness (mm).
5.	Insulin Level: Serum insulin (mu U/ml).
6.	BMI: Body mass index (weight in kg/(height in m)^2).
7.	Diabetes Pedigree Function: A score indicating the likelihood of diabetes based on family history.
8.	Age: Age of the patient (years).
9.	Outcome: Class variable (1 for diabetes, 0 for non-diabetes).
    
 Model Training and Evaluation
•	Each model was trained using the training dataset.
•	Performance was evaluated using the test dataset, with metrics calculated as follows:
1.	Confusion Matrix: Provides a summary of prediction results.
2.	Accuracy: The ratio of correct predictions to total predictions.
3.	Precision: The ratio of true positive predictions to the total predicted positives.
4.	Recall: The ratio of true positive predictions to actual positives.
5.	F1-Score: The harmonic means of precision and recall, providing a single metric for model performance.

Modeling and Algorithms in my project are:
•	Tree Model (40%): Given its perfect AUC score, it should have the most focus in your evaluation and analysis.Its accuracy 95.1%.
•	SVM (30%): As the second-best performer, it deserves significant attention. Its accuracy 86.4%.
•	KNN (20%): While it also achieved a perfect AUC, the focus here is on understanding its specific contributions. Its accuracy 80.8%
•	Logistic Regression (10%): With a poor performance, this model should be reviewed to understand its limitations. Its accuracy 79.5%

Analysis of Performance Metrics
1.	Tree Model: The perfect AUC suggests that the decision tree model can perfectly distinguish between the classes. High recall indicates that most positive cases are correctly identified, but the F1 score suggests that it may not be making positive predictions, leading to a lack of precision. This could be a sign of overfitting or an imbalance in the dataset.
2.	KNN Model: The model's high precision suggests that when it predicts a positive case, it is often correct. However, its recall indicates that it misses some actual positive cases, which may be critical in a medical context.
3.	Logistic Regression Model: This model provided a good balance between precision and recall, making it a reliable choice for early diabetes prediction. Its performance indicates that it can effectively assist healthcare professionals in identifying at-risk patients.
4.	SVM Model: Although the SVM model showed a higher recall (86.4%), this was at the cost of precision and accuracy. The lower precision indicates that many negative cases were incorrectly classified as positive, which could lead to unnecessary anxiety for patients.
   
 Feature Importance
Analysis of feature importance revealed that glucose levels and BMI were among the most significant indicators for predicting diabetes. This aligns with existing medical literature, emphasizing the importance of these metrics in diabetes risk assessment. The Diabetes Pedigree Function also emerged as a significant predictor, highlighting the role of family history in diabetes risk.

Conclusion
This project successfully demonstrates the application of machine learning techniques in predicting diabetes. The KNN and Logistic Regression models were identified as the most effective approaches, while the SVM model highlighted the importance of balancing recall and precision in medical predictions. The insights gained from this analysis provide valuable information for healthcare professionals in early diagnosis and intervention strategies.

References
https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset
