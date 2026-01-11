# 🧠 Brain Tumor Detection & Segmentation with Deep Learning

The project revolves around the development of a high-performance algorithm for analyzing brain tumor MRI scans. By automating the detection and segmentation processes, the model supports clinicians by reducing their workload and enhancing diagnostic accuracy.

Accurate segmentation of medical images is critical for improving clinical decision-making and patient outcomes, particularly in complex cases involving brain tumors. This work explores how modern deep learning models can assist radiologists by quickly and consistently identifying tumor regions in MRI images.

---

## 📊 Dataset

- Public brain MRI dataset  
- 100+ patients  
- 256×256 image slices  
- Each image includes a tumor mask annotated by radiologists  
- Data split into training, validation, and test sets  

Class imbalance was addressed using stratified sampling and data augmentation.

---

## 🧠 Models

Three deep learning models were evaluated:

- **U-Net** – purpose-built for image segmentation  
- **ResNet-50** – transfer learning with residual connections  
- **VGG-19** – transfer learning from image classification  

All models were trained using Dice loss and evaluated on segmentation and classification metrics.

---

## 🏆 Results

| Model | Dice | IoU | Binary Acc | Precision | Recall | F1 |
|------|------|-----|------------|-----------|--------|----|
| **ResNet-50** | **0.899** | **0.819** | **0.998** | 0.964 | 0.964 | 0.964 |
| **U-Net** | 0.863 | 0.763 | 0.997 | 0.947 | 0.947 | 0.947 |
| U-Net (Optuna) | 0.834 | 0.720 | 0.997 | 0.931 | 0.931 | 0.931 |
| VGG-19 | 0.758 | 0.614 | 0.995 | 0.816 | 0.768 | 0.774 |

ResNet-50 achieved the strongest overall performance, while U-Net offered an excellent balance of accuracy and computational efficiency.

---

## 👨‍💼 My Role

- Clinical background research  
- Model evaluation and tuning  
- Results analysis  
- Technical writing and presentation  
- Team collaboration and reviews  

---

## 🛠️ Tech Stack

Python • TensorFlow/Keras • OpenCV • NumPy • Pandas • Optuna • Jupyter  

---