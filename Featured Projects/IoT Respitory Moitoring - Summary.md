# 🌬️ IoT-Based Respiratory Monitoring with Deep Learning

This project explores how Internet of Things (IoT) systems and machine learning can be used to monitor respiratory patterns and support the management of conditions such as sleep apnea and asthma.

By combining real-time sensor data with deep learning models, the system aims to improve patient monitoring, support telemedicine workflows, and provide clinicians with clearer insights into breathing behavior.

---

## ☁️ System Overview

The proposed system integrates:

- Respiratory and pressure sensors  
- Edge devices for local data capture  
- Secure cloud storage and processing  
- Deep learning models for prediction  
- A dashboard for clinician review  

This architecture supports continuous monitoring while maintaining data security and reliability.

---

## 📊 Data

- Public respiratory sensor dataset  
- 80 adult patients  
- Millions of time-series measurements  
- Includes flow rate, tidal volume, pressure, and movement signals  
- Patient demographics and asthma labels  

The data was segmented into short time windows for model training and evaluation.

---

## 🧠 Models

Two main deep learning approaches were used:

- **LSTM** for learning temporal breathing patterns  
- **CNN + LSTM** for extracting features from spectrograms and modeling time dependencies  

Models were trained to predict:

- Flow rate  
- Tidal volume  
- Asthma classification  

---

## 🏆 Results

- CNN + LSTM slightly improved prediction accuracy over LSTM alone  
- Personalized (patient-specific) models outperformed generalized models  
- Asthma classification showed moderate performance due to class imbalance  

The results demonstrate the potential of deep learning for respiratory monitoring, while highlighting the importance of personalized modeling in healthcare applications.

---

## 📈 Visualization & Dashboard

A Tableau dashboard was created to display:

- CPAP usage trends  
- Breathing performance over time  
- Tidal volume summaries  
- Patient compliance indicators  

This supports telemedicine workflows and clinician–patient communication.

---

## 👨‍💼 My Role

- System design and architecture  
- Data analysis and visualization  
- Model evaluation  
- Dashboard development  
- Research and documentation  

---

## 🛠️ Tech Stack

Python • TensorFlow/Keras • CNN • LSTM  
Pandas • NumPy • Tableau  
MQTT • Cloud IoT concepts  

