# No-Show Appointments Prediction

## Project Overview

This project aims to predict whether patients will attend their scheduled medical appointments by analyzing historical, demographic, and behavioral data. Accurate predictions help healthcare providers reduce missed appointments, optimize scheduling, and improve overall service efficiency.

The problem is framed as a binary classification task, with the target variable indicating if a patient showed up or not. Key features include patient age, gender, health conditions, previous no-show behavior, financial aid status, and reminder notifications.

## Technical Approach

We implemented and compared several machine learning models to address this problem, including:

- **XGBoost:** Handles complex patterns with strong performance on imbalanced data.
- **Ridge Regression:** Provides a regularized linear modeling baseline.
- **Naive Bayes:** Offers a probabilistic baseline model.

Models were evaluated using cross-validation and performance metrics suitable for imbalanced datasets, such as recall (sensitivity), specificity, precision, G-Mean, accuracy, and AUC.

## Dataset

The dataset contains 72,607 appointment records with 18 features, capturing demographic, behavioral, and clinical attributes related to patient attendance at medical appointments in Espírito Santo, Brazil. The target variable is binary, indicating if the patient showed up (`Yes` or `No`).

## Key Insights & Recommendations

- Patients with a history of missed appointments are high-risk and should be targeted with personalized outreach (e.g., reminders, follow-ups).
- Reducing waiting times can decrease no-show rates by optimizing scheduling and staffing.
- Multi-channel communication strategies (SMS, phone calls, emails) outperform SMS reminders alone.
- Flexible rescheduling and transportation support can help remove attendance barriers.
- Continuous monitoring and adaptive strategies improve appointment adherence over time.
- Association rule mining (market basket analysis) can reveal patterns linked to no-shows, aiding in identifying high-risk profiles.

## Computing Requirements

The models were trained on a standard machine with 8GB RAM and multi-core CPU. For scalability and faster training (especially with XGBoost), cloud resources were occasionally utilized.

## How to Use

1. Clone the repository.
2. Prepare the dataset as per the data schema.
3. Run data preprocessing scripts.
4. Train and evaluate models using the provided Jupyter notebooks.
5. Use the trained model to predict no-shows on new patient data.

## Author
SaiPranayTummala
