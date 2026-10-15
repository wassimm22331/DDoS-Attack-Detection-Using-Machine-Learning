# DDoS Attack Detection Using Machine Learning

Machine learning project for detecting **Distributed Denial-of-Service (DDoS) attacks in Industrial IoT environments** from network and MQTT traffic.

The project covers the complete workflow from raw network data preparation to feature engineering, model training and evaluation.

---

## Project Overview

Industrial IoT systems rely heavily on connected devices and communication protocols such as MQTT, making them vulnerable to network attacks.

The objective of this project was to build a machine learning pipeline capable of distinguishing between:

- **Benign network traffic**
- **Malicious / DDoS traffic**

The final processed dataset contained approximately **988,000 network records**.

---

## Workflow

The project follows several stages:

1. Raw PCAP and JSON traffic processing
2. Conversion of network data into structured CSV format
3. Data cleaning and preprocessing
4. Feature engineering
5. Exploratory data analysis
6. Machine learning model training
7. Model comparison
8. Performance evaluation

A Streamlit-based utility was also developed to facilitate the conversion of **PCAP / JSON network data into CSV format**.

---

## Dataset

The processed dataset contained approximately:

**987,890 observations**

The data was divided into training and testing sets containing both benign and malicious network traffic.

### Main information used

The dataset includes information related to:

- Timestamps
- Source devices
- IP addresses
- MAC addresses
- Applications
- MQTT message information
- MQTT QoS
- MQTT message type
- MQTT topics
- Duplicate messages
- Retained messages

The target variable represents:

```text
0 → Benign traffic
1 → Malicious traffic
