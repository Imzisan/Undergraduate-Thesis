# 🧠 Bangla Handwritten Character Detection using Custom Loss Function

This repository contains the implementation of our **undergraduate thesis project** titled  
**“Bangla Handwritten Character Detection using Custom Loss Function”**,  
submitted to the **Department of Computer Science and Engineering**,  
**American International University–Bangladesh (AIUB)** in January 2024.

---

## 📘 Overview
Bangla is a widely used language with a complex handwritten script, which poses challenges for accurate character recognition.  
This project explores **deep learning** and **transfer learning** techniques to improve recognition accuracy by introducing a  
**custom dynamic regularization loss function** — designed to balance model precision and generalization.

Our research aims to enhance early stopping, reduce overfitting, and improve adaptability in deep neural network training.

---

## 🚀 Objectives
- Develop an effective model for **Bangla handwritten character recognition**.  
- Implement a **custom loss function** with dynamic regularization for adaptive training.  
- Compare the proposed method against **Categorical Cross-Entropy Loss**.  
- Analyze model performance using various **CNN architectures**.

---

## 🧩 Methodology
### 1. Transfer Learning
We utilized pre-trained CNN models as feature extractors to enhance learning efficiency:
- **VGG16**
- **MobileNetV2**
- **ResNet50**
- **DenseNet201**
- **InceptionV3**
- **VGG19**
- **Xception**

### 2. Custom Dynamic Regularization Loss
We introduced a **Dynamic Regularization Loss Function** that modifies the regularization strength during training:
Total Loss(ytrue, ypred, t) = CrossEntropy(ytrue, ypred) + Dynamic Strength(t) × L2 Regularization

This helps maintain a balance between **accuracy** and **generalization** through adaptive regularization.

### 3. Dataset
Bangla handwritten dataset containing isolated characters and numerals  
(pre-processed and augmented for model robustness).

---

## ⚙️ Tools & Technologies
- **Python 3**
- **TensorFlow / Keras**
- **NumPy, Pandas, Matplotlib**
- **OpenCV**
- **Google Colab / Jupyter Notebook**

---

## 📊 Results Summary
- The proposed **custom loss function** improved generalization compared to categorical cross-entropy.  
- **VGG16** and **MobileNetV2** models achieved stable validation accuracy with reduced overfitting.  
- Demonstrated that **dynamic regularization** helps optimize early stopping during training.

| Model | Loss Function | Validation Accuracy | Notes |
|--------|----------------|--------------------|-------|
| VGG16 | Cross-Entropy | 79.96% | Overfitting observed |
| VGG16 | Custom Loss | 71.62% | Better training stability |
| MobileNetV2 | Cross-Entropy | 45.88% | Low generalization |
| MobileNetV2 | Custom Loss | 69.23% | Significant improvement |

---



---

## 🧠 Key Takeaways
- Dynamic regularization improves **adaptability** and **training efficiency**.
- Demonstrated an effective **loss function optimization** strategy for CNN-based handwriting recognition.
- Potential applications in **OCR**, **document digitization**, and **AI language systems**.

---

## 👥 Authors
- **Md. Sakib Hossain Zisan** — 18-37823-2  
- **Sumit Kanti Sarker** — 19-41764-3  
- **Nesar Uddin** — 19-41759-3  
- **Abu Naser Md Abu Sadik** — 19-39912-1  

**Supervisor:**  
*Dr. Debajyoti Karmaker, Associate Professor, Department of Computer Science, AIUB.*

---

## 📄 Thesis Document
📘 [Download Full Thesis (PDF)](./Formatted%20Book.pdf)

---

## 🏁 Acknowledgment
We sincerely thank our supervisor, peers, and the Department of Computer Science at **AIUB** for their guidance, support, and feedback throughout the research.

---

## 📬 Contact
For any queries or collaboration:  
📧 **sakibhossainzisan@gmail.com**  
🔗 [LinkedIn](https://www.linkedin.com/in/imzisan/)

---

### ⭐ If you found this project useful or interesting, don’t forget to give it a star on GitHub!

