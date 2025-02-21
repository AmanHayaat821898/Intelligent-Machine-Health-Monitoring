# Intelligent Machine Health Monitoring

## 1. Overview

---

This project focuses on developing a web application for predictive maintenance utilizing the AI4I 2020 Predictive Maintenance Dataset. The application integrates machine learning models to:

Predict whether equipment is at risk of failure based on process parameters like air and process temperature, rotational speed, torque, and tool wear.

Classify the type of failure when one occurs, leveraging the same set of parameters.


[https://github.com/praj2408/Predictive-Maintenance-System-Monitoring/assets/70437673/863a61cf-14bc-43aa-937e-823edcb4d1b2](https://github.com/user-attachments/assets/87fb60a3-43e6-4461-bad2-d56d14a1393a)


## 2. Motivation

---

Predictive maintenance is crucial for industries seeking to optimize operations, minimize downtime, and reduce repair costs. By deploying an AI-driven system, users gain real-time insights into equipment performance, enabling proactive maintenance actions to prevent unexpected failures.

## 3. Success Metrics

---

The success of this project will be evaluated based on:

Model Performance: Precision, recall, and F1-score of the predictive models.

User Experience: Application responsiveness and ease of use.

Impact: Reduction in downtime and maintenance expenses.

## 4. Requirements & Constraints

---

### 4.1 Functional Requirements

Users must be able to input process parameters and receive failure predictions.

The application should provide insights into the model's performance metrics.

Data visualization features should allow users to analyze equipment 

### 4.2 Non-functional Requirements

The model should achieve high precision, recall, and F1-score.

The web app should be user-friendly, responsive, and secure.

### 4.3 Constraints

- The system should be built using Streamlit for the frontend.

Deployment will be done using Docker and Hugging Face Spaces.

Cost-effective deployment is a priority.

### 4.4 Out-of-scope

Integration with third-party applications or external data sources.

Advanced diagnostic reports beyond failure prediction.

## 5. Methodology

---

### 5.1. Problem Statement
The primary challenge is to develop a machine learning-based system that can reliably predict equipment failures and classify failure types based on given parameters.

### 5.2. Data

The dataset consists of 50,000+ records with 14 features, including operational parameters like air/process temperature, rotational speed, torque, and tool wear.

The target variable is a binary indicator of failure occurrence.

### 5.3. Techniques

The project will utilize:

Binary classification for failure prediction.

Multi-class classification for failure type identification.

Key steps in the ML pipeline include:

Data preprocessing (handling missing values, feature scaling, encoding categorical features).

Feature engineering and selection.

Model training and hyperparameter tuning.

Performance evaluation and testing.

## 6. Architecture

---

The application consists of multiple components:

Frontend: A Streamlit-based web interface for user interaction.

Backend: API services to handle model inference and data processing.

Machine Learning Model: Responsible for failure prediction and classification.

Deployment: Docker containers encapsulate the application, hosted on Hugging Face Spaces.

CI/CD Pipeline: Automated workflows using GitHub Actions ensure continuous integration and deployment.

## 7. Pipeline

---

The end-to-end machine learning pipeline follows these steps:

Data Input: Users upload datasets or enter process parameters.

Preprocessing: Data is cleaned, transformed, and prepared for model training.

Model Training & Evaluation: Multiple models are trained, tuned, and compared.

Containerization: The complete application is packaged into a Docker container.

Cloud Deployment: The application is deployed on Hugging Face Spaces for accessibility.

User Interaction: Users access the web application to get real-time predictions.

Prediction Storage & Analysis: Predictions are logged for future evaluation and improvements.

Continuous Integration & Deployment: Automated updates ensure seamless improvements and model retraining.

`Web App`: The web application is accessible via a web browser, providing a user-friendly interface for interacting with the prediction functionality. Users can input new data and obtain predictions from the deployed model.

`Prediction`: The deployed model uses the input data from the web application to generate predictions. These predictions are then displayed to the user via the web interface.

`Data`: The predicted data is captured and stored, providing a record of the predictions made by the web application. This data can be used for analysis, monitoring, or further processing as needed.

`CI/CD Pipeline`: The pipeline is automated using GitHub Actions, which allows for continuous integration and deployment of the application. This automation ensures that the application is always up-to-date and provides a consistent experience for users.
