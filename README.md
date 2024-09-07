# Diabetes-Prediction-Model

This project focuses on developing a predictive model for diabetes using a dataset that includes various health metrics such as glucose level, blood pressure, BMI, age, and more. By employing machine learning techniques, we aim to accurately predict the likelihood of an individual having diabetes based on these features. The dataset is first preprocessed to handle missing values and then split into training and testing sets. Various algorithms, including Random Forest, Logistic Regression, Decision Trees, and Support Vector Machines, are evaluated using GridSearchCV to find the best performing model. The chosen model is then validated and its performance is assessed using accuracy scores and confusion matrices. This project not only demonstrates the application of machine learning in healthcare but also provides valuable insights into the factors contributing to diabetes, ultimately aiding in early diagnosis and better management of the disease.

## Visualization of Diabetes Outcomes

This bar plot illustrates the distribution of diabetes outcomes within the dataset. The x-axis represents whether individuals have diabetes (0 for no, 1 for yes), while the y-axis shows the count of individuals in each category. The plot reveals that there are more individuals without diabetes compared to those with diabetes, as evidenced by the taller bar on the left. This visualization helps in understanding the dataset's imbalance, with a higher number of non-diabetic individuals. The plot has been customized by removing the top and right spines for a cleaner appearance.
![image](https://github.com/user-attachments/assets/041fe229-efbb-4cf8-aaec-85b6e0ddace7)

## Data Cleaning 
The dataset contained several invalid zero values in key features like Glucose, BloodPressure, SkinThickness, Insulin, and BMI. Since these medical measurements cannot be zero, these values were replaced with `NaN` to mark them as missing data. To handle the missing data, we analyzed the distribution of each feature through histograms. Based on this analysis, we filled missing values using statistical measures: the mean was used for Glucose and BloodPressure, while the median was used for SkinThickness, Insulin, and BMI, as their distributions were skewed. This process ensured the dataset was clean and ready for further analysis and modeling.


![image](https://github.com/user-attachments/assets/01243ae1-5451-47f2-93ee-7519c98411a0)

## Model Performance Evaluation

The model was evaluated using confusion matrices on both the training and test datasets. The confusion matrices show the performance of our Random Forest Classifier in predicting whether a person has diabetes.

Test Set Confusion Matrix:
The matrix shows 272 true negatives and 123 true positives, with only 5 false negatives and 0 false positives. This indicates a strong ability to correctly classify both diabetic and non-diabetic cases in the test data.

Training Set Confusion Matrix:
The model performed nearly perfectly on the training data, with 1044 true negatives and 555 true positives, and only 1 false negative. The absence of false positives highlights the model's high accuracy.

The overall accuracy achieved on the test set was 98.75%, and the training set accuracy was 99.94%, showing excellent performance with minimal overfitting.
![image](https://github.com/user-attachments/assets/d8d4aab7-9e93-4d38-a043-13070591ab55)

![image](https://github.com/user-attachments/assets/22f9a12d-782d-405c-a6bb-2ad4566f2262)


![image](https://github.com/user-attachments/assets/a6f72e2f-588e-43e4-8de9-7def32daab64)

![image](https://github.com/user-attachments/assets/9b8272fe-a66d-402c-9a13-b8c7cb44e364)





