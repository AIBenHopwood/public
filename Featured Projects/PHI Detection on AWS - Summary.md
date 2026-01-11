# 🔒 PHI Detection & De-Identification for Clinical Text

This project focuses on developing an AI system to automatically detect and remove Protected Health Information (PHI) from clinical documents. By automating the de-identification process, the system helps protect patient privacy while enabling safer use of medical text for research, analytics, and AI development.

Because the project involved sensitive healthcare data, all model training and data storage were hosted in a **secure AWS environment** with a **VPN-based private network** to align with HIPAA-style security and privacy requirements.

---

## ☁️ Secure Cloud Infrastructure (AWS)

To ensure data protection and regulatory alignment, the system was deployed using a private AWS environment:

- Virtual Private Cloud (VPC) with restricted network access  
- VPN for secure remote connections  
- Encrypted S3 storage for clinical text data  
- Isolated compute instances for model training  
- Controlled IAM access policies  

This setup ensured that sensitive data was never exposed to public networks and followed healthcare-style security practices.

---

## 📊 Dataset

- Clinical discharge summaries derived from the MIMIC-IV dataset  
- Synthetic PHI injected to avoid exposure to real patient identifiers  
- 20+ PHI entity types (e.g., names, dates, locations, hospitals)  
- BIO-tagged for token-level classification  
- Split into training, validation, and test sets  

Synthetic data was used to maintain privacy while enabling realistic model training.

---

## 🧠 Model

The primary model used was **ClinicalBERT**, a transformer pretrained on medical text and fine-tuned for Named Entity Recognition (NER).

- Token-level PHI classification  
- BIO tagging scheme  
- Optimized with AdamW  
- Fine-tuned for clinical language patterns  

A traditional BiLSTM model was also evaluated but performed significantly worse than the transformer-based approach.

---

## 🏆 Results

The ClinicalBERT model achieved very high performance on the synthetic evaluation dataset:

- Precision ≈ 1.00  
- Recall ≈ 1.00  
- F1 ≈ 1.00  

Confusion matrices showed strong separation between PHI and non-PHI tokens.

### Important Note on Evaluation

These results should be interpreted with caution due to:

- Heavy use of synthetic data  
- Repeated PHI patterns  
- Template-based clinical notes  
- Potential overlap between training and test distributions  

The project emphasizes **secure system design, privacy protection, and real-world applicability** over raw metric values.

---

## 👨‍💼 My Role

- Designed secure AWS training environment  
- Configured VPN and private network access  
- Managed encrypted data storage  
- Evaluated PHI detection models  
- Analyzed data leakage risks  
- Framed system for HIPAA-style compliance  
- Led technical documentation and presentation  

---

## 🛠️ Tech Stack

Python • PyTorch • Hugging Face Transformers • ClinicalBERT  
AWS (VPC, EC2, S3, IAM, VPN)  
Pandas • NumPy • SeqEval  
