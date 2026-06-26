📌 Project Overview
HYBRID AI-POWERED NETWORK INTRUSION DETECTION & ANOMALY DETECTION SYSTEM
Overview

This project presents an AI-powered Hybrid Network Intrusion Detection System (NIDS) that leverages Machine Learning techniques to identify malicious network activities and distinguish them from legitimate network traffic. The system analyzes network connection features from the NSL-KDD dataset and predicts whether incoming traffic is normal or an attack.

Multiple machine learning algorithms are implemented and compared to identify the best-performing model for intrusion detection. The trained model is deployed through a Flask web application, enabling users to interact with the prediction system through a simple web interface.

🎯 Objectives
Detect malicious network traffic using Machine Learning.
Differentiate between normal and attack network connections.
Compare multiple machine learning algorithms based on their performance.
Reduce false-positive and false-negative predictions.
Deploy the trained model using Flask for real-time prediction.
Visualize model performance using graphs and evaluation metrics.
🚀 Key Features
AI-powered Network Intrusion Detection
Multiple Machine Learning Algorithms
Data Preprocessing and Feature Engineering
High Accuracy Classification
Model Performance Comparison
Confusion Matrix Visualization
ROC Curve Analysis
Feature Importance Analysis
Saved Machine Learning Model (.pkl)
Flask-based Web Application
Easy-to-use Prediction Interface
🧠 Machine Learning Algorithms
Logistic Regression

A linear classification algorithm used as a baseline model for binary intrusion detection.

Advantages
Fast training
Simple implementation
Good baseline performance
Decision Tree

A tree-based supervised learning algorithm that classifies network traffic based on decision rules.

Advantages
Easy to understand
Handles nonlinear relationships
Feature importance support
Random Forest

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting. It achieved the best overall performance and was selected as the final deployment model.

Advantages
High accuracy
Robust against overfitting
Handles large datasets efficiently
XGBoost

Extreme Gradient Boosting is an optimized ensemble algorithm known for high predictive performance and computational efficiency.

Advantages
High accuracy
Excellent handling of complex data
Faster training than many ensemble methods
Support Vector Machine (SVM)

Support Vector Machine identifies the optimal decision boundary to separate normal and malicious network traffic.

Advantages
Effective for high-dimensional data
Good classification performance
Strong generalization capability
K-Nearest Neighbors (KNN)

KNN classifies a network connection by comparing it with its nearest neighboring samples.

Advantages
Easy implementation
No training phase
Suitable for small datasets
📊 Dataset
NSL-KDD Dataset

The NSL-KDD dataset is a benchmark cybersecurity dataset widely used for intrusion detection research. It contains both normal and malicious network traffic records with multiple network-related features.

The dataset eliminates redundant records found in the original KDD Cup 1999 dataset and provides a balanced evaluation environment.

Dataset Features

Examples include:

Duration
Protocol Type
Service
Flag
Source Bytes
Destination Bytes
Wrong Fragment
Logged In
Count
Destination Host Count
Same Service Rate
Destination Host Service Count

Total Features:

41 Input Features

Target Variable:

Normal / Attack

Data Preprocessing

The preprocessing stage includes:

Handling categorical variables
Label Encoding
Feature Scaling
Train-Test Split
Feature Selection
⚙️ Project Workflow
NSL-KDD Dataset
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Train Machine Learning Models
        │
        ▼
Performance Evaluation
        │
        ▼
Best Model Selection
        │
        ▼
Model Deployment using Flask
🏗️ System Architecture
Data Collection

Network traffic data is collected from the NSL-KDD dataset.

Data Preprocessing

Categorical attributes are encoded and numerical features are normalized for model training.

Feature Engineering

Relevant features are selected and transformed into machine learning-ready data.

Model Training

Six machine learning algorithms are trained and evaluated.

Model Evaluation

Models are compared using standard evaluation metrics.

Flask Deployment

The best-performing model is integrated into a Flask application for interactive predictions.

📈 Model Evaluation

The following evaluation metrics are used:

Accuracy
Precision
Recall
F1 Score
ROC-AUC Score
Confusion Matrix

Generated Visualizations:

Model Accuracy Comparison
Confusion Matrix
ROC Curve
Feature Importance Graph
📂 Project Structure
HYBRID-NETWORK-INTRUSION-DETECTION-SYSTEM
│
├── app
│   ├── templates
│   │   └── index.html
│   └── app.py
│
├── data
│   ├── KDDTrain+.txt
│   └── KDDTest+.txt
│
├── models
│   └── random_forest.pkl
│
├── notebooks
│   └── EDA.ipynb
│
├── reports
│   ├── model_comparison.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
├── src
│   ├── preprocessing.py
│   ├── train_models.py
│   └── evaluate_models.py
│
├── requirements.txt
├── README.md
└── LICENSE
💻 Installation
Clone Repository
git clone https://github.com/your-username/HYBRID-NETWORK-INTRUSION-DETECTION-SYSTEM.git
Create Virtual Environment
python -m venv venv
Activate Environment

Windows

venv\Scripts\activate

Linux/macOS

source venv/bin/activate
Install Dependencies
pip install -r requirements.txt
▶️ Running the Project
Train the Models
jupyter notebook

Open:

EDA.ipynb

Run all notebook cells.

Launch Flask Application
python app/app.py
Access Web Interface

Open your browser:

http://127.0.0.1:5000
🛠️ Technologies Used
Programming Language
Python
Machine Learning
Scikit-learn
XGBoost
Data Processing
Pandas
NumPy
Data Visualization
Matplotlib
Seaborn
Web Framework
Flask
Development Tools
Jupyter Notebook
Visual Studio Code
Git
GitHub
📷 Project Screenshots

Include the following images:

Flask Home Page
Model Accuracy Comparison
Confusion Matrix
ROC Curve
Feature Importance
📊 Results
Successfully trained six machine learning algorithms.
Random Forest achieved the best overall performance.
High classification accuracy on the NSL-KDD dataset.
Successfully deployed the trained model using Flask.
Generated comprehensive evaluation reports and visualizations.
🔮 Future Enhancements
Real-Time Network Traffic Monitoring
Deep Learning-based Intrusion Detection
Zero-Day Attack Detection
Cloud Deployment
REST API Integration
Docker Containerization
Real Packet Capture Analysis
SIEM Integration
