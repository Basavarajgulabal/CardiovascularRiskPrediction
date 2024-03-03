Cardiovascular Risk Prediction
https://camo.githubusercontent.com/79b9ebf559ab32fe7c42f98b5592fc8170dae4a606579fce07137dea04536a6e/68747470733a2f2f737465616d75736572696d616765732d612e616b616d616968642e6e65742f7567632f313937333136393932323934313239393939392f413442354644343537354530464339353133413139343241463842333835333146434337343937412f3f696d773d36333726696d683d33353826696d613d66697426696d706f6c6963793d4c6574746572626f7826696d636f6c6f723d253233303030303030266c6574746572626f783d74727565
This project aims to predict the 10-year risk of developing coronary heart disease (CHD) using the Cardiovascular Risk Prediction dataset. The dataset contains information on 3,390 individuals with 16 predictor variables and 1 target variable. The variables represent potential demographic, behavioral, and medical risk factors.

Problem Statement
The classification goal is to predict whether a patient has a 10-year risk of CHD. Given the dataset's attributes and patient information, we need to develop a machine learning model that accurately predicts the likelihood of developing CHD.

Summary
The Cardiovascular Risk Prediction dataset provides detailed information on patients' demographics, behaviors, and medical risk factors. In this project, we tackled the challenge of predicting the 10-year risk of developing coronary heart disease by implementing a machine learning pipeline.

Here is a summary of our approach and key steps:

1 -Data Gathering and Cleaning: We started by gathering the dataset, which contains over 4,000 records and 15 attributes. We performed data cleaning, handling null values, checking data distribution, and handling outliers to ensure data quality.

2-Exploratory Data Analysis (EDA): In this phase, we conducted an in-depth analysis of the dataset. We employed various visualization techniques, separating them into univariate, bivariate, and multivariate categories. Through EDA, we gained meaningful insights that guided our decision-making for the subsequent steps.

3-Feature Engineering and Preprocessing: We performed feature engineering to extract new features that could potentially impact the prediction of the 10-year CHD risk. Additionally, we addressed multicollinearity among independent variables using the Variance Inflation Factor (VIF). Categorical features were encoded into numerical values using binary label encoding.

4-Data Transformation: To achieve normally distributed data, we applied various transformation techniques such as logarithmic, exponential, and square root transformations. We also visualized the quantile-quantile plot to assess the distance from the normal distribution. Additionally, we employed the StandardScaler from the sklearn library to scale the data.

5-Handling Imbalanced Dataset: The distribution of the target variable, TenYearCHD, was found to be imbalanced, with only 15% of individuals classified as having a high risk of developing CHD. To address this issue, we employed the Synthetic Minority Oversampling Technique (SMOTE) to create a balanced dataset.

6-Model Selection and Evaluation: We split the data into train and test sets, ensuring stratified samples of both classes. We evaluated several classification models, including Logistic Regression, Random Forest, XGBoost, Naive Bayes, KNN, and SVM. Various metrics such as Precision, Recall, F1 Score, Accuracy, and AUC-ROC were compared using classification reports and confusion matrices. Considering our objective of reducing false negatives, emphasizing Recall was essential. After thorough experimentation, XGBoost emerged as the optimal model, achieving the highest metrics overall.

7-Model Deployment: Based on our evaluations and comparisons, we selected XGBoost as our final model for deployment. This model, fine-tuned with a learning rate of 0.1, maximum tree depth of 5, and 350 trees, demonstrated superior Recall, Precision, F1 Score, Accuracy, and AUC-ROC scores.

In conclusion, this project presented an extensive exploration of the Cardiovascular Risk Prediction dataset, employing various machine learning techniques to predict the 10-year risk of developing coronary heart disease. By combining data processing, feature engineering, model evaluation, and selection, we successfully built an accurate model capable of identifying potential CHD patients in the future.





