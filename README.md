# Diabetes Predictor | XGBoost vs Random Forest

This machine learning project utilizes diagnostic measures to predict whether a patient has diabetes. Featuring models like XGBoost and Random Forest, the code evaluates their predictive performance on a dataset of clinical diabetes measures.

## Dataset Overview
The dataset includes the following features with a binary outcome indicating the presence of diabetes:
- Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age

Missing values in `Glucose`, `SkinThickness`, `Insulin`, and `BMI` are imputed using median values. The dataset was balanced using SMOTE to address class imbalance.

## Model Training and Evaluation
After preprocessing, including scaling features and addressing class imbalance:
- **Random Forest** and **XGBoost** classifiers were trained.
- Hyperparameter tuning was performed using GridSearchCV.
- The best parameters were extracted for both models.

## Results Summary
- Random Forest achieved an accuracy of **80%**.
- XGBoost achieved a slightly lower accuracy of **77.5%**.
- The best model was saved as `XGboost_diabetes_model.joblib`.

Random Forest outperformed XGBoost in this scenario, potentially due to better handling of the dataset's characteristics or the effect of hyperparameter settings.

## Usage
To replicate the analysis:
1. Balance the dataset with SMOTE.
2. Split the data into training and test sets.
3. Scale the features.
4. Train models using the provided hyperparameters.
5. Evaluate using accuracy, precision, recall, and F1 score.

For more details, see the provided Jupyter notebooks and scripts.

## Contact
For inquiries or contributions, please contact spomar36@gmail.com.


# Production Services

To ensure our diabetes prediction model operates seamlessly in a production environment, we leverage the following cloud services and ML operations practices:

## AWS
- **Amazon S3**: Store and retrieve any amount of data at any time.
- **AWS Lambda**: Run code in response to data changes in S3 buckets.
- **Amazon SageMaker**: Train, tune, and deploy the machine learning models.

## Azure
- **Azure Blob Storage**: For large-scale data storage.
- **Azure Functions**: Event-driven compute for data processing.
- **Azure Machine Learning Service**: Build, train, and deploy models.

## GCP
- **Google Cloud Storage**: Durable and scalable object storage.
- **Cloud Functions**: Serverless execution of functions in response to cloud events.
- **AI Platform**: End-to-end machine learning model lifecycle management.

## ML Operations
- **Continuous Training**: Implement pipelines to retrain models with new data.
- **Data Validation**: Use services like AWS Data Pipeline or Azure Data Factory for data integrity checks.
- **Model Monitoring**: Track model performance and data drift to maintain accuracy over time.

These services ensure our model stays updated, scalable, and maintainable, with robust ML operations that support continuous improvement.

Quickstart:

git clone https://github.com/GOSS-hash/boosting-algorithms-project-tutorial-omass/tree/main
cd [Your Repository Directory]
