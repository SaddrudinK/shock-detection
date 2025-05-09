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
