# OPTIMIZING-ARTIFICIAL-NEURAL-NETWORK-A-COMPARITIVE-STUDY-IN-COMBAT-VEHICLES
# Overview

This project develops a machine learning-based Remaining Useful Life (RUL) prediction system to improve predictive maintenance for aerospace and maritime assets.
It processes real-time telemetry and historical maintenance data to accurately forecast the time before critical failures, reducing downtime, optimizing maintenance schedules, and improving operational safety.

We evaluate both a standalone Artificial Neural Network (ANN) model and a hybrid Random Forest + ANN model to achieve highly accurate, robust predictions.

# Key Features

📈 Real-Time Prediction using telemetry data (temperature, pressure, vibration, etc.)

🛠 Data Preprocessing: missing value handling, outlier removal, normalization

🧠 Advanced Modeling:

Standalone ANN for nonlinear pattern learning

Hybrid Random Forest + ANN for enhanced robustness and interpretability

📊 Model Interpretability with SHAP analysis and feature importance extraction

🚀 Real-Time Deployment using scalable cloud/edge architectures

🔄 Continuous Learning: automatic model updates with new data

# Dataset
The system uses:

Telemetry Data: Sensor readings such as temperature, pressure, vibration, rotation speed

Maintenance Logs: Historical repairs, part replacements, servicing records

Failure Events: Recorded incidents of breakdowns and component failures

Data is structured and stored in CSV or relational databases for easy access during preprocessing and training.

System Architecture
Data Collection Module
Real-time ingestion via APIs / Kafka / MQTT, combined with historical data import.

Preprocessing Module
Data cleaning, normalization (Min-Max scaling, Z-score), outlier detection.

Feature Engineering
Extraction of statistical metrics, temporal trends, and degradation patterns.

Predictive Modeling
Training of ANN and Hybrid models using hyperparameter tuning and cross-validation.

Real-Time Inference
Deployment for live RUL predictions and maintenance planning.

Visualization and Reporting
Time-series analysis, SHAP explanations, trend visualizations.

# Model Performance

Model	                 Accuracy      	Precision	      Recall	      F1 Score
ANN                    	96.19%	        0.709	         0.949        	0.812
Random Forest + ANN	     96.7%	        0.758	          0.915	        0.822
✅ Hybrid model outperforms standalone ANN across all key metrics.

Technologies Used
Python 3.10+

TensorFlow / Keras (for ANN)

Scikit-learn (for Random Forest, preprocessing, metrics)

Pandas, NumPy (for data handling)

Matplotlib, Seaborn (for visualization)

SHAP (for model interpretability)

Apache Kafka / MQTT (for real-time data ingestion)

Docker (optional: containerized deployment)

