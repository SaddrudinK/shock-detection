# Pediatric Hemodynamic Shock Prediction Challenge

## Overview
This repository contains my solution to the **Pediatric Hemodynamic Shock Prediction Challenge** on Kaggle. The goal of the competition is to develop machine learning models that predict the onset of hemodynamic shock in critically ill pediatric patients within six hours, using a synthetic dataset representing real-world PICU (Pediatric Intensive Care Unit) scenarios.

## Objective
In pediatric intensive care units, timely recognition of hemodynamic instability—or shock—is critical for patient outcomes. This challenge focuses on predicting the onset of shock, enabling early intervention and improving patient outcomes.

### Competition Goals:
- Develop predictive models that can identify the onset of shock at least six hours before clinical deterioration.
- The evaluation is based on the **F1 Score**, which is appropriate for the class imbalance problem in this competition (shock vs. no-shock).

## Data Overview
The dataset includes the following:
- **Physiological parameters** (e.g., heart rate, blood pressure, oxygen saturation)
- **Laboratory results**
- **Clinical markers**
- **Target variable**: `shock_within_6h`, indicating whether a patient will experience shock within six hours.

## Approach

### Tools Used:
- **AI-powered tools** and **starter books** helped in getting started and guiding through the process.
- Primarily used **XGBoost** for classification tasks, given its efficiency in handling imbalanced data.
- Data preprocessing steps included:
  - Handling missing values
  - Feature engineering
  - Normalization

### Models Used:
- Tried multiple models to achieve the best performance:
  - **Logistic Regression**
  - **Random Forest**
  - **XGBoost**
- Hyperparameter tuning was performed to optimize the performance of each model.

### Current Status:
- **Current Ranking**: As of now, I am ranked **5th** on the **public leaderboard**. The ranking is based on performance on the public test set, and the final ranking will depend on the private test set after the competition ends.

## Submission Format:
The submission file format follows the exact structure required by Kaggle:
```csv
patient_id,shock_within_6h
PICU_IYINNC,1
PICU_D7NKJF,0
PICU_DYGH15,0
PICU_RP5NBF,0
...

## Folder Structure:
/notebooks         # Jupyter notebooks for data exploration and modeling
/data              # Contains data files (or links to download them)
/output            # Output files (predictions, logs, etc.)
/models            # Saved models (if applicable)
requirements.txt   # List of Python dependencies

## Requirements
To run this project, you'll need to install the required Python packages. You can do this by running:

pip install -r requirements.txt

Required Libraries:
- numpy: For numerical computing and array manipulation.
- pandas: For data manipulation and analysis.
- scikit-learn: For building machine learning models and preprocessing.
- xgboost: A powerful gradient boosting model for classification tasks.
- matplotlib: For creating static, animated, and interactive visualizations.
- seaborn: For statistical data visualization.

## Running the Code
1. Clone this repository:
git clone https://github.com/SaddrudinK/shock-detection.git

2. Navigate to the project folder:
cd shock-detection

3. Open the Jupyter notebook and run the cells:
jupyter notebook

The notebook contains the following steps:
- Data loading and preprocessing.
- Exploratory data analysis (EDA).
- Model building and evaluation.
- Prediction generation.

#Feel free to reach out if you have any questions or suggestions for improvements!
