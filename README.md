Intrusion Detection Using ML
Advanced Intrusion Detection System using Machine Learning (CICIDS2017)
 Executive Summary
This project applies Machine Learning (ML), Decision Trees, and Neural Networks to develop an Intrusion Detection System (IDS) capable of identifying cyber threats such as DDoS, Port Scans, and Web Attacks. Using the CICIDS2017 dataset (2.8M+ records, 79 features), this study tackles cybersecurity challenges with a data-driven approach.
Objective
✔ Build a scalable, automated IDS for real-time cyber threat detection.
✔ Overcome traditional systems' limitations in handling high-volume, complex network traffic.
✔ Apply Decision Trees & Neural Networks to detect anomalies & rare attack patterns.
Key Achievements
 97% Accuracy with Decision Tree model for common attacks (SYN Flag Count).
 Neural Network outperformed for rare attacks like SQL Injection & Web Attacks.
 Data Optimization: Chunked processing (10,000 rows) prevented memory crashes.
 Feature Engineering: Addressed missing values, outliers, and class imbalances.
 Dataset Overview (CICIDS2017)
Dataset
Size
Features
Attack Types
CICIDS2017
2.8M+ records
79
DDoS, PortScan, Botnet, SQL Injection, Brute Force
Key Features: Flow Duration, Packet Length, Flag Counts, Flow Bytes/s.
Challenges: Data imbalance, large size (causing crashes), missing values, and high dimensionality.
Methodology
1. Data Processing & Cleaning
Chunked Processing: Processed 10K rows at a time to prevent system crashes.
Imputation: Replaced missing values (Median for Flow Bytes/s, IQR for outlier removal).
Feature Selection: Used correlation analysis & heatmaps to optimize features.
Class Imbalance Handling: Applied SMOTE (Synthetic Minority Oversampling Technique).
2. Model Development
2.1. Decision Tree Model
Achieved 97% accuracy for common attacks.
Identified important features: SYN Flag Count, Flow Duration, Fwd Packets.
Strengths: High interpretability, fast performance.
Weaknesses: Struggled with rare attacks.
2.2. Neural Network Model (Optimized)
Initial Accuracy: 0.196 → Optimized Accuracy: 0.324
Performed better for rare attack detection (SQL Injection, Web Attacks).
Optimizations:
Increased neurons per layer, added dropout layers for overfitting control.
Adjusted batch size to 64 for model stability.
Increased epochs to 50 to refine learning.

Weakness: Computationally expensive, still requires class balance improvements.
Data Visualizations
1. Correlation Heatmap
Highlights correlation between Flow Duration, Packet Length, and SYN Flag Count.
Key Insight: High correlation allows feature reduction to improve model efficiency.
2. Class Distribution (Bar Chart)
Class Imbalance: BENIGN class dominates (~75%), rare attacks are underrepresented.
Solution: Applied SMOTE to balance dataset & improve model recall.
3. Decision Tree Feature Importance
Top Features: Flow Duration, SYN Flag Count, Total Fwd Packets.
Insight: These features are highly predictive for intrusion detection.
Business Impact
1. Scalable, Automated IDS for Real-Time Cyber Threat Detection
Enhances Security Operations: Automates cyber threat detection, reducing manual monitoring.
Faster Response to Threats: Identifies attacks in real-time, allowing Security Operations Centers (SOCs) to mitigate risks immediately.
Prevents Data Breaches: Early detection stops attackers before they compromise sensitive data.
2. Overcome Traditional Systems' Limitations in Handling High-Volume, Complex Network Traffic
Handles Big Data Efficiently: Optimizes processing large-scale network traffic without crashes.
Improves Threat Visibility: ML-based IDS detects Advanced Persistent Threats (APTs).
Reduces False Positives: Unlike traditional IDS, ML models learn from network behavior, preventing unnecessary alerts.
3. AI-Powered Threat Detection
Reduces Security Gaps: Many companies fail to detect low-frequency but high-risk threats (SQL Injection, Web Attacks).
AI-Powered Adaptability: The system learns from network behavior and adapts to new attack patterns.
Enhances Network Resilience: Helps CISOs & SOC teams focus on high-risk alerts instead of manual log analysis.
Final Model Performance
Model
Accuracy
Strengths
Weaknesses
Decision Tree
97%
Fast, interpretable, effective for common attacks
Poor recall for rare attacks
Neural Network
32% (Optimized)
Effective for rare attacks (SQL Injection, Web Attacks)
Computationally expensive, requires better class balancing
Best Approach: Hybrid Model (combining Decision Tree, Neural Network, and Gradient Boosting) to improve recall and optimize class balancing.
References
DataCamp: Decision Tree Classification in Python
ScikitLearn: Neural Networks in Python
Kaggle: CICIDS2017 Dataset Cleaning
UNB Cybersecurity Research: CIC IDS Datasets
Project Links
GitHub Repository: Network Anomaly Detection
Portfolio Website: Danielle's Portfolio
LinkedIn: Danielle Bopda

