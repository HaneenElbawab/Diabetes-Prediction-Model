# Diabetes-Prediction-Model
# Problem Statement:
This project aims to develop a predictive model that accurately determines whether a patient has diabetes based on the dataset obtained from Kaggle.

# Dataset:
The dataset consists of medical records and diagnostic measurements, with features that help in predicting diabetes. Since the dataset is imbalanced, handling this imbalance effectively is crucial.

# Model Selection:
For this project, I used the Random Forest algorithm because it efficiently handles imbalanced data and provides robust predictions. Random Forest is an ensemble learning method that reduces overfitting and improves accuracy by combining multiple decision trees.

# Model Results:
After applying Random Forest with optimized hyperparameters, the model achieved the following results:
Accuracy: 77%
Precision for Class 1 (Diabetic): 0.63
Recall for Class 1 (Diabetic): 0.82
The model performed well in identifying diabetic patients (high recall), but it sometimes misclassified non-diabetic individuals as diabetic (lower precision).

# Challenges & Solutions:
Imbalanced Data:
Used class_weight={0:1, 1:2} in Random Forest to give more importance to the minority class.
Considered resampling techniques like SMOTE to generate synthetic samples for class 1.
Improving Precision:
Tried threshold tuning to balance precision and recall.
Experimented with different algorithms like XGBoost and Logistic Regression to compare results.
Feature Engineering:
Performed data cleaning and scaling to enhance model performance.

# Future Work:

Experiment with deep learning models like Neural Networks.
Implement more advanced resampling methods.
Fine-tune hyperparameters further for better generalization.

Random Forest was chosen due to its ability to handle imbalanced data efficiently. The model achieved good recall, making it useful for detecting diabetic cases. However, improvements in precision are needed, which can be addressed through further experimentation with different techniques.
