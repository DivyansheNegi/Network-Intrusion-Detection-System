# Network-Intrusion-Detection-System
* This is a machine learning–based Network Intrusion Detection System designed to classify and detect cyber threats.  
* Developed using IBM Cloud and Watson Studio (Watson AI), it identifies network intrusions such as Denial-of-Service (DoS) and Probe attacks.  
* The project analyzes labeled network traffic data to distinguish between normal activity and potential security threats.
* This system is built using automated machine learning, making it  efficient, scalable, and well-suited for real-world cybersecurity applications.

# Dataset

* Source: [Kaggle – Network Intrusion Detection](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)
* Format: CSV
* Target: class column indicating normal or attack types.
* Features: Include duration, protocol type, service, flag, source/destination bytes, and many more.

# Model used

* Decision Tree: A traditional, interpretable model suitable for classification tasks.
* Snap Decision Tree: A variation of the traditional Decision Tree algorithm, optimized for faster execution and simplified decision-making while maintaining similar classification logic.

# Model Workflow

This section outlines the full end-to-end process used to build and evaluate the model:

1. Data upload and schema detection  
2. Preprocessing and feature engineering  
3. Model experimentation using various algorithms  
4. Automatic pipeline selection based on validation scores  
5. Evaluation and export of best-performing model

![Model Workflow](images/progress_map.png)


# Model Architecture Insights

The system intelligently connects components such as data transformers, feature selectors, and model evaluators.  
It also incorporates a 3-fold cross-validation approach along with a separate holdout set for final model assessment.  
This architecture ensures a clean, modular pipeline that is scalable and easy to reuse for similar machine learning tasks.

![Model Architecture](images/relationship_map.png)


# Evaluation

Model performance was assessed using cross-validation across several key metrics:
* Accuracy
* Precision
* Recall
* F1-Score
* Log Loss
* ROC-AUC
These metrics helped in identifying the most balanced and robust model for intrusion detection.

![Model Evaluation Metrics](images/metric_chart.png)

# Result

The model was deployed using IBM Watson Studio and tested on real network traffic data. Below is the output of the binary classification system, identifying whether the traffic is normal or an anomaly based on the model’s predictions.

![Model Prediction Results](images/results.png)


# Disclaimer

* The dataset used in this project belongs to its original creators on Kaggle. This repository uses the dataset solely for educational and research purposes.
