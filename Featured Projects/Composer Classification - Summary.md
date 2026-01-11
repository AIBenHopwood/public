# 🎵 Composer Classification with Deep Learning

This project focuses on classifying classical music compositions by composer using deep learning. By analyzing MIDI files, the system learns musical patterns that distinguish between composers such as Bach, Beethoven, Chopin, and Mozart.

The goal was to explore how sequence-based and convolutional neural networks can capture both temporal structure and stylistic features in music.

---

## 📊 Data

- Public MIDI dataset of classical music  
- Four composers: Bach, Beethoven, Chopin, Mozart  
- Each file converted into note sequences and musical features  
- Data augmented using pitch shifting to improve generalization  
- Class imbalance addressed with oversampling  

The preprocessing pipeline transformed raw MIDI files into model-ready numerical representations.

---

## 🧠 Models

Two deep learning approaches were evaluated:

- **LSTM** – for learning temporal note sequences  
- **CNN** – for detecting musical patterns and motifs  

Both models were trained and optimized using:

- Data augmentation  
- Regularization  
- Hyperparameter tuning with Optuna  

---

## 🏆 Results

- CNN achieved the highest overall accuracy  
- LSTM performed well on sequential patterns  
- Data augmentation improved generalization  
- Hyperparameter tuning significantly boosted performance  

<img width="1977" height="2381" alt="Model Comparison" src="https://github.com/user-attachments/assets/2d9f687f-0357-4a69-b835-857cb0b19c5f" />



The models successfully learned stylistic differences between composers based on musical structure.


Hypertuing was reasonably successful:
<img width="715" height="591" alt="tuning" src="https://github.com/user-attachments/assets/d6acf5d3-4014-4c1f-b3db-feae0b358347" />


---

## 👨‍💼 My Role

- Data preprocessing and cleaning  
- Feature extraction from MIDI files  
- Model implementation (LSTM & CNN)  
- Hyperparameter tuning  
- Results analysis and documentation  

---

## 🛠️ Tech Stack

Python • TensorFlow/Keras • CNN • LSTM  
music21 • mido • Optuna  
Pandas • NumPy  
