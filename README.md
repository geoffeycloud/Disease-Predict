Heart Disease Prediction Project
Project Description
This project aims to predict the likelihood of heart disease based on patient data using machine learning techniques. We explore different classification models and evaluate their performance.

Data Source
The dataset used in this project is the Heart Disease UCI dataset, obtained from Kaggle Hub. It contains various patient attributes that are used as features for the prediction models.

Methodology
The project follows these steps:

Data Loading: Load the Heart Disease UCI dataset into a pandas DataFrame.
Data Cleaning: Handle missing values in the dataset by filling numeric columns with the mean and categorical columns with 'Unknown'.
Preprocessing:
Convert boolean columns to integers.
Perform one-hot encoding on categorical features.
Align columns with the training data to ensure consistency.
Scale the numerical features using StandardScaler.
Model Training:
Train a Logistic Regression model.
Train a Random Forest Classifier model.
Model Evaluation:
Evaluate the models using metrics such as accuracy, classification report, and confusion matrix.
Analyze feature importance for the Random Forest model.
Model Saving: Save the trained Random Forest model and the scaler object using joblib for future use.
Prediction on New Data: Provide a method to upload new data (in a specified format) and obtain heart disease predictions using the saved model and scaler.
Results
Both Logistic Regression and Random Forest models were trained and evaluated. The Random Forest model generally showed better performance based on the evaluation metrics. Feature importance analysis was conducted to identify the most influential features in the Random Forest model.

How to Run the Notebook
Upload Kaggle API Key: Follow the initial steps in the notebook to upload your kaggle.json file and set up the Kaggle environment.
Install Kaggle Hub: Ensure the kagglehub library is installed (already included in the notebook).
Run Cells: Execute the code cells sequentially. This will download the dataset, perform data preprocessing, train and evaluate models, save the model, and prepare for user prediction.
User Upload and Prediction: Use the provided cells to upload a CSV file with new patient data (following the Heart_user_template.csv format) and get predictions.
File Structure
heart_rf_model.pkl: Saved Random Forest model.
heart_scaler.pkl: Saved StandardScaler object.
Heart_user_template.csv: A template CSV file showing the expected format for user prediction data
