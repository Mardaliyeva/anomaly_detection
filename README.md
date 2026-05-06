# anomaly_detection
Unsupervised Anomaly Detection on network traffic data using Isolation Forest. The project analyzes CICIDS2017 flow-based cybersecurity dataset to identify abnormal network behavior without using labeled data. Includes data preprocessing, feature engineering, visualization, and anomaly detection modeling.

# 🛡️ Network Anomaly Detection using Machine Learning

This project focuses on detecting abnormal network traffic patterns using **unsupervised machine learning** techniques. The model is trained on the CICIDS2017 dataset and identifies anomalies without using labeled attack data during training.

---

## 📌 Project Goal

To build a system that can:
- Learn normal network behavior
- Detect unusual or suspicious traffic patterns
- Work without relying on labeled data during training

---

## 📊 Dataset

:contentReference[oaicite:0]{index=0}

The dataset contains network flow statistics such as:
- Flow duration
- Packet sizes
- Packet rates
- Time-based features
- TCP flag information

Each row represents a network flow with extracted statistical features.

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Removed redundant features (high correlation filtering)
- Handled numerical feature scaling using StandardScaler

### 2. Feature Engineering
- Selected network flow-based statistical features
- Removed highly correlated variables (corr > 0.9)

### 3. Model
:contentReference[oaicite:1]{index=1}

- Unsupervised anomaly detection algorithm
- Builds random trees to isolate rare patterns
- Anomalies are easier to isolate than normal points

### 4. Evaluation (Without Labels)
Since this is an unsupervised problem:
- Anomaly score distribution
- Visual inspection (PCA plots)
- Anomaly ratio analysis
- Domain-based interpretation

---

## 📈 Visualizations

The project includes:
- Distribution plots of network features
- Boxplots for outlier detection
- Correlation heatmaps
- PCA-based anomaly visualization
- Scatter plots of detected anomalies

---

## 🧠 Key Insight

Anomalies are detected based on:
- Unusual traffic volume
- Irregular packet timing
- Extreme values in flow duration
- Imbalanced forward/backward traffic patterns

---

## 🚀 Results

- Successfully identifies rare and unusual network patterns
- Detects anomalies without labeled training data
- Provides interpretable anomaly scoring

---

## 📂 Project Structure
