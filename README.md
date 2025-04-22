# Algerian_Forest_fire_prediction

![alt text](Algerian_Forest.jpg)

🧱 Project Architecture Diagram

The project follows a modular structure, integrating data processing, machine learning, and web deployment components

┌────────────────────────────┐
│        User Interface      │
│  (HTML/CSS via Flask)      │
└────────────┬───────────────┘
             │
             ▼
┌────────────────────────────┐
│       Flask Web Server     │
│        (app.py)            │
└────────────┬───────────────┘
             │
             ▼
┌────────────────────────────┐
│     Model Prediction       │
│  (Ridge Regression Model)  │
│    (model.pkl)             │
└────────────┬───────────────┘
             │
             ▼
┌────────────────────────────┐
│   Data Preprocessing       │
│ (StandardScaler object)    │
│    (scaler.pkl)            │
└────────────┬───────────────┘
             │
             ▼
┌────────────────────────────┐
│      Dataset Input         │
│  (Algerian Forest Fires)   │
└────────────────────────────┘


🔄 Workflow Diagram

The workflow encompasses data handling, model training, and deployment phases:​

1. Data Collection:
   - Obtain Algerian Forest Fires dataset.

2. Data Preprocessing:
   - Clean and preprocess data.
   - Feature selection and scaling using StandardScaler.

3. Model Training:
   - Train Ridge Regression model on preprocessed data.
   - Evaluate model performance (e.g., R² score).

4. Model Serialization:
   - Save trained model as 'model.pkl'.
   - Save scaler object as 'scaler.pkl'.

5. Web Application Development:
   - Develop Flask application (application.py).
   - Create HTML templates for user input and result display.

6. Deployment:
   - Deploy Flask app to a web server (e.g., AWS Elastic Beanstalk ).
   - Users input data via web interface to get predictions.