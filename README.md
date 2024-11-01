
# Coronary Heart Disease Prediction Using Machine Learning

This project develops a machine learning-based predictive model for identifying individuals at risk of coronary heart disease (CHD) using data from the 2021 Behavioral Risk Factor Surveillance System (BRFSS). The analysis employs various machine learning algorithms, addressing class imbalance through undersampling, oversampling, and SMOTE techniques, with an ensemble approach for optimal predictive performance.

## Table of Contents
- Project Overview
- Dataset
- Methodology
- Models Implemented
- Technologies Used
- Setup and Installation
- Usage
- Results


## Project Overview
Coronary heart disease (CHD) is a leading cause of mortality globally, making early detection crucial for patient outcomes. This study applies advanced machine learning techniques to predict CHD risk by analyzing demographic, health, and lifestyle factors. Results demonstrate the potential of machine learning models in identifying high-risk individuals, thus enabling timely interventions.

## Dataset
The dataset used for this study is the **Behavioral Risk Factor Surveillance System (BRFSS) 2021**. This dataset provides health-related information from over 400,000 participants across the United States, capturing a range of factors such as age, gender, income, health metrics (e.g., BMI, blood pressure), and lifestyle behaviors (e.g., smoking, physical activity).

### Key Variables
- **Demographic Information**: Age, gender, race, education level, income.
- **Health Metrics**: BMI, high blood pressure, cholesterol levels, diabetes, history of heart attacks and strokes.
- **Lifestyle Factors**: Smoking, alcohol use, physical activity.
- **Outcome Variable**: Presence or absence of coronary heart disease.

## Methodology
1. **Data Preprocessing**: Cleaning, handling missing values, encoding categorical variables, and normalizing numerical features.
2. **Exploratory Data Analysis (EDA)**: Analyzed age, gender, and health distributions; identified correlations among variables.
3. **Feature Selection**: Used correlation analysis and Variance Inflation Factor (VIF) to select the most predictive features.
4. **Imbalanced Data Handling**: Applied techniques like SMOTE, oversampling, and undersampling to address class imbalance.
5. **Model Training**: Employed various machine learning algorithms, with cross-validation and hyperparameter tuning for optimization.
6. **Evaluation Metrics**: Accuracy, precision, recall, F1-score, and ROC-AUC were used to evaluate model performance.

## Models Implemented
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost**
- **Voting Classifier (Ensemble Method)**

## Technologies Used
- **Python**: Core programming language.
- **Scikit-learn**: For machine learning model building.
- **Imbalanced-learn**: For resampling techniques.
- **XGBoost**: Gradient boosting for enhanced performance.
- **Matplotlib and Seaborn**: Data visualization.
- **Streamlit**: For creating the application interface.

## Setup and Installation

1. Clone the repository:
   git clone https://github.com/your-username/chd-prediction.git
   
2. Navigate to the project directory:
   cd chd-prediction
   
3. Install the required packages:
   pip install -r requirements.txt
   


## Usage
1. **Data Preparation**: Place the BRFSS 2021 dataset in the specified directory or modify the code to read from the correct path.
2. **Run Model Training**: Execute the notebook or script to preprocess data, train models, and evaluate performance.
3. **Streamlit Interface**: If using Streamlit, launch the interface to interact with the model and make predictions.

## Results
The ensemble models, particularly the Voting Classifier with Logistic Regression and XGBoost, demonstrated strong predictive accuracy. Key insights include:
- High accuracy and ROC-AUC scores were achieved, with logistic regression and XGBoost performing robustly on balanced data.
- Ensemble methods showed improved precision and recall, validating the effectiveness of combining models for CHD prediction.
