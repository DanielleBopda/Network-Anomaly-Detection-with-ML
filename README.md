** Advanced Intrusion Detection System using Machine Learning (CICIDS2017)**



** Project Overview**

This project applies Machine Learning (ML), Decision Trees, and Neural Networks to develop an Intrusion Detection System (IDS) capable of identifying cyber threats such as DDoS, Port Scans, and Web Attacks. Using the CICIDS2017 dataset (2.8M+ records, 79 features), this study aims to enhance real-time cyber threat detection for improved network security.


Objective

Develop an AI-powered Intrusion Detection System (IDS) for real-time cyber threat detection.Overcome traditional IDS limitations by handling large-scale network traffic efficiently.Apply Decision Trees and Neural Networks to detect anomalies and rare attack patterns.


Dataset Overview

Name: CICIDS2017 (Canadian Institute for Cybersecurity Intrusion Detection System dataset).

Size: 2.8M+ network traffic records.

Features: 79, including Flow Duration, Packet Length, Flag Counts, and Flow Bytes/s.

Attack Types:

DDoS

Port Scans

Botnet Attacks

SQL Injection

Brute Force Attacks



** Methodology**

1. Data Processing & Cleaning

Chunked Processing: Processed 10K rows at a time to prevent system crashes. Imputation: Replaced missing values (e.g., median for Flow Bytes/s). Feature Engineering: Correlation analysis & heatmaps for feature selection. Class Imbalance Handling: Applied SMOTE (Synthetic Minority Oversampling Technique).


2. Model Development


a. Decision Tree Model

Achieved 97% accuracy for common attacks.Identified important features: SYN Flag Count, Flow Duration, Fwd Packets.Strengths: Fast & interpretable.Weaknesses: Struggled with rare attacks like SQL Injection.


b. Neural Network Model (Optimized)

Initial Accuracy: 0.196 → Optimized Accuracy: 0.324Performed better for rare attack detection (SQL Injection, Web Attacks).Optimizations:

Increased neurons per layer, added dropout layers for overfitting control.

Adjusted batch size to 64 for model stability.

Increased epochs to 50 for better learning.



** Data Visualizations**


1. Correlation Heatmap

Highlights key features like Flow Duration, Packet Length, and SYN Flag Count.

Helps reduce unnecessary features and improve model efficiency.


2. Class Distribution (Bar Chart)

Identifies imbalance in attack vs. benign traffic.

Used SMOTE to generate synthetic attack samples & improve recall.


3. Decision Tree Feature Importance

Key Predictors: Flow Duration, SYN Flag Count, Total Fwd Packets.

Helps in prioritizing critical network features.



** Business Impact**


1. Scalable, Automated IDS for Real-Time Cyber Threat Detection

 Automates cyber threat detection, reducing manual monitoring efforts. Enables faster response to network attacks in Security Operations Centers (SOCs). Prevents data breaches by detecting intrusions before they escalate.


2. Overcoming Traditional IDS Limitations

 Handles big data efficiently, preventing memory crashes in high-volume network traffic. Improves threat visibility, detecting Advanced Persistent Threats (APTs). Reduces false positives compared to rule-based systems.


3. AI-Powered Anomaly Detection

 Identifies rare attack patterns like SQL Injection & Web Attacks.Learns from network behavior, adapting to new cyber threats.Helps CISOs & SOC teams focus on high-risk alerts instead of manual log analysis.



** Final Model Performance**

Model

Accuracy

Strengths

Weaknesses

Decision Tree

97%

Fast, interpretable, detects common attacks

Poor recall for rare attacks

Neural Network

32% (Optimized)

Detects rare attacks (SQL Injection, Web Attacks)

Computationally expensive, requires class balancing

 Best Suggestion for alternative models: Hybrid Model (Decision Tree + Neural Network + Gradient Boosting) to enhance overall performance.



Project Links

GitHub Repository: Network Anomaly Detection
Portfolio Website: Danielle's Portfolio
LinkedIn: Danielle Bopda


     
