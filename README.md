# Alzheimer's Disease Diagnosis Prediction

This project aims to predict Alzheimer's Disease diagnosis based on various health, lifestyle, and clinical features. We implemented and tested several machine learning models to classify whether a patient is diagnosed with Alzheimer's Disease (Yes/No). Among the models used, Gradient Boosting delivered the highest accuracy, achieving 98%. Further improvements were made by applying feature scaling techniques such as StandardScaler to enhance the model's performance.

## Dataset
### Patient ID
- PatientID: A unique identifier assigned to each patient
### Demographic Details
- Age: The age of the patients ranges from 60 to 90 years.
- Gender: Gender of the patients (Male or Female)
- Ethnicity: The ethnicity of the patients Caucasian; African American; Asian; Other
- EducationLevel: The education level of the patients, None; High School; Bachelor's; Higher
### Lifestyle Factors
- BMI: Body Mass Index of the patients, ranging from 15 to 40.
- Smoking: Smoking status, where 0 indicates No and 1 indicates Yes.
- AlcoholConsumption: Weekly alcohol consumption in units, ranging from 0 to 20.
- PhysicalActivity: Weekly physical activity in hours, ranging from 0 to 10.
- DietQuality: Diet quality score, ranging from 0 to 10.
- SleepQuality: Sleep quality score, ranging from 4 to 10.
### Medical History
- FamilyHistoryAlzheimers: Family history of Alzheimer's Disease, where 0 indicates No and 1 indicates Yes.
- CardiovascularDisease: Presence of cardiovascular disease, where 0 indicates No and 1 indicates Yes.
- Diabetes: Presence of diabetes, where 0 indicates No and 1 indicates Yes.
- Depression: Presence of depression, where 0 indicates No and 1 indicates Yes.
- HeadInjury: History of head injury, where 0 indicates No and 1 indicates Yes.
- Hypertension: Presence of hypertension, where 0 indicates No and 1 indicates Yes.
### Clinical Measurements
- SystolicBP: Systolic blood pressure, ranging from 90 to 180 mmHg.
- DiastolicBP: Diastolic blood pressure, ranging from 60 to 120 mmHg.
- CholesterolTotal: Total cholesterol levels, ranging from 150 to 300 mg/dL.
- CholesterolLDL: Low-density lipoprotein cholesterol levels, ranging from 50 to 200 mg/dL.
- CholesterolHDL: High-density lipoprotein cholesterol levels, ranging from 20 to 100 mg/dL.
- CholesterolTriglycerides: Triglycerides levels, ranging from 50 to 400 mg/dL.
### Cognitive and Functional Assessments
- MMSE: Mini-Mental State Examination score, ranging from 0 to 30. Lower scores indicate cognitive impairment.
- FunctionalAssessment: Functional assessment score, ranging from 0 to 10. Lower scores indicate greater impairment.
- MemoryComplaints: Presence of memory complaints, where 0 indicates No and 1 indicates Yes.
- BehavioralProblems: Presence of behavioral problems, where 0 indicates No and 1 indicates Yes.
- ADL: Activities of Daily Living score, ranging from 0 to 10. Lower scores indicate greater impairment.
### Symptoms
- Confusion: Presence of confusion, where 0 indicates No and 1 indicates Yes.
- Disorientation: Presence of disorientation, where 0 indicates No and 1 indicates Yes.
- PersonalityChanges: Presence of personality changes, where 0 indicates No and 1 indicates Yes.
- DifficultyCompletingTasks: Presence of difficulty completing tasks, where 0 indicates No and 1 indicates Yes.
- Forgetfulness: Presence of forgetfulness, where 0 indicates No and 1 indicates Yes.
## Diagnosis Information
- Diagnosis: Diagnosis status for Alzheimer's Disease, where 0 indicates No and 1 indicates Yes.

## Data Preprocessing
Before training the models, we performed the following preprocessing steps:

- Handling Missing Values: Filled missing values with the median of the respective columns.
- Label Encoding: Converted categorical values such as gender (Male = 1, Female = 0) and smoking status (Yes = 1, No = 0).
- Feature Scaling: Applied StandardScaler to normalize the data and ensure better model performance, especially for algorithms sensitive to feature scaling.

### Machine Learning Models
We tested the following machine learning models to predict Alzheimer's Disease diagnosis:

- Logistic Regression
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Gradient Boosting
Each model's performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.

Out of all the models, Gradient Boosting emerged as the best performing model with an accuracy of 98%. The model effectively captured complex patterns in the data and outperformed other models in terms of both accuracy and consistency.

## Future Enhancements
- Feature Engineering: Further refining the dataset by exploring new features and interaction terms could improve model accuracy.
- Hyperparameter Tuning: We can perform grid search or randomized search for better hyperparameter optimization across different models.
- Ensemble Methods: Exploring ensemble learning techniques such as stacking multiple models might further improve accuracy.
- Advanced Scaling Techniques: In addition to StandardScaler, other scaling methods (e.g., MinMaxScaler) could be tested to further enhance performance.
