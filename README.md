# Student Dropout Prediction Using Machine Learning and Deep Learning Techniques: A Comparative Analysis of XGBoost and Multilayer Perceptron

# Problem Statement
Student dropout is a major challenge for educational institutions because it affects academic performance, institutional reputation, graduation rates and the efficient use of educational resources. Students who leave their studies before completion often experience reduced career opportunities, while institutions incur financial losses and lower retention rates.

Traditional methods of identifying students at risk of dropping out rely on manual monitoring by lecturers or academic advisors. These approaches are often less reactive, time-consuming and may fail to detect students who require support at an early stage.

Advances in machine learning provide an opportunity to analyze large volumes of student data and identify patterns associated with dropout risk. By considering multiple factors—including academic performance, attendance, financial stress, lifestyle behaviors and psychological well being predictive model can identify students who are likely to drop out before the problem becomes critical.

This project was therefore undertaken to develop and evaluate machine learning and deep learning models capable of predicting student dropout risk. The ultimate goal is to support educational institutions in implementing data-driven early intervention strategies that improve student retention and academic success.

# Project Objective
# General Objective
To develop and evaluate a machine learning model that predicts student dropout risk using demographic, academic, financial, lifestyle and psychological factors.

# Specific Objectives
Explore factors that are associated with student dropout.

To build and compare machine learning and deep learning models for dropout prediction.

To optimize the best-performing model using hyperparameter tuning.

To identify the most influential factors affecting student dropout.

# Metodology

<img width="362" height="559" alt="Screenshot (168)" src="https://github.com/user-attachments/assets/33d502b1-02c4-456b-9f80-627da1cb4692" />

# Results
The performance of the developed models was evaluated using accuracy, precision, recall and F1-score. 

Accuracy: 0.75
              precision    recall  f1-score   support

           0       0.77      0.64      0.70        73
           1       0.74      0.84      0.78        87

    accuracy                           0.75       160
   macro avg       0.75      0.74      0.74       160
weighted avg       0.75      0.75      0.75       160

Confussion Metrix

[[47 26]
 [14 73]]

The baseline Multilayer Perceptron (MLP) achieved an accuracy of 69%, while the baseline XGBoost model improved the accuracy to 69.4%. After hyperparameter tuning using GridSearchCV, the XGBoost model achieved the best performance with an accuracy of 75%.

The tuned XGBoost model produced the following results:

Metric Score Accuracy 75% Precision 74% Recall 84% F1-score 78%

<img width="1037" height="547" alt="image" src="https://github.com/user-attachments/assets/7d259a33-a724-45e8-8a11-70fa66936c6b" />

Feature importance analysis identified burnout level, year of study, attendance percentage, family income bracket and age as the most influential factors in predicting student dropout.

# Discussion
The results demonstrate that the tuned XGBoost model outperformed the deep learning model, indicating that tree-based algorithms are more effective for this structured tabular dataset. Hyperparameter tuning significantly improved model performance, increasing the accuracy from 69.4% to 75%.

The feature importance analysis revealed that burnout level was the strongest predictor of student dropout, followed by academic factors such as attendance percentage and year of study as well as socioeconomic factors such as family income bracket. These findings suggest that student dropout is influenced by a combination of psychological, academic and financial factors.

The model's 84% recall for the dropout class indicates that it can successfully identify most students who are at risk of dropping out, making it suitable as an early warning tool to support timely interventions by educational institutions.

# Conclusion
This study developed and evaluated machine learning and deep learning models to predict student dropout using demographic, academic, financial, lifestyle and psychological factors. Among the evaluated models, the tuned XGBoost classifier achieved the best performance, with an accuracy of 75%, demonstrating that it is well suited for structured educational data.

Feature importance analysis showed that burnout level was by far the most influential predictor of student dropout. Both Low Burnout and Medium Burnout were among the highest-ranked features, indicating that student well-being plays a central role in predicting dropout risk. Academic factors such as year of study, attendance percentage and study hours per day also contributed substantially to the model, while financial and lifestyle variables, including family income, social activity, screen time, exercise frequency and stress level, further improved predictive performance.

These findings suggest that student dropout is influenced by a combination of academic performance, mental well-being, financial circumstances and lifestyle behaviors rather than by a single factor. The model therefore provides a practical tool for identifying students who may require early academic or personal support.

# Recommendations
Prioritize student well-being
Burnout was the most influential predictor, institutions should strengthen mental health services by providing counseling, stress management programs and regular well-being assessments.

Monitor student attendance
Attendance was strongest academic predictors. Institutions should implement attendance monitoring systems that alert academic advisors when attendance declines so that support can be provided before students disengage.

Support students during critical years of study
Year of study suggests that dropout risk varies across different stages of a degree program. Institutions should identify years with higher dropout rates and provide targeted mentoring and academic support during those periods.

Provide financial support
Because family income contributed to the model, institutions should consider expanding scholarships, emergency financial assistance and flexible payment options for students experiencing financial difficulties.

Promote healthy study and lifestyle habits
Study hours, exercise frequency and screen time were all meaningful predictors. Universities should encourage balanced study schedules, regular physical activity as well as healthy technology use through student development programs.

Encourage student engagement
Social activity was identified as an important feature, indicating that connected students may have better persistence. Institutions should promote student organizations, mentoring programs and peer-support initiatives.

Implement an early warning system
The tuned XGBoost model can be integrated into institutional systems to identify students with a high predicted dropout risk. Advisors can then use these predictions to initiate timely academic, financial or psychological interventions.
