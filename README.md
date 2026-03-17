# 🩺 Handling Multi-Class Imbalance in Breast Ultrasound Image Classification (BUSI)

A complete deep learning experimental pipeline to classify **Breast Ultrasound Images** into three classes — **Benign, Malignant, and Normal** — with a strong research focus on **handling class imbalance** and improving **minority class performance**.

This repository systematically compares multiple imbalance handling strategies and analyzes their effectiveness using **Recall, Macro-F1 Score, and Confusion Matrix**.

---

## 📌 Project Motivation

Medical imaging datasets frequently suffer from **severe class imbalance**, where some clinically critical classes have very few samples. Standard training approaches often result in models that achieve high overall accuracy but perform poorly on minority classes.

This project builds a **structured experimental framework** to:

- Evaluate different imbalance handling techniques  
- Improve detection of minority classes  
- Perform fair comparison using robust evaluation metrics  
- Provide research insights for medical image classification  

---

## 🎯 Objectives

- Perform **3-class classification** on the BUSI dataset  
- Improve **minority class recall**
- Compare multiple imbalance handling strategies  
- Analyze **Macro-F1 performance**
- Build a **reproducible deep learning pipeline**

---

## 📂 Dataset

- **Dataset:** BUSI (Breast Ultrasound Images Dataset)  
- **Task:** Multi-class Image Classification  

### Classes

- Benign  
- Malignant  
- Normal  

The dataset shows **significant imbalance** across classes, making it ideal for experimentation with imbalance learning strategies.

---

## ⚙️ Imbalance Handling Techniques Compared

### ✅ Baseline  
Standard CNN training without any imbalance handling.

### ✅ Data Augmentation  
- Random Horizontal Flip  
- Rotation  
- Zoom  
- Intensity Variations  

### ✅ Weighted Sampling  
Class-balanced sampling during mini-batch training.

### ✅ Focal Loss  
Down-weights easy samples and focuses training on difficult/minority samples.

### ✅ SMOTE Hybrid Strategy  
Synthetic oversampling of minority class features combined with deep learning training.

### ✅ Mixup Regularization  
Linear interpolation between samples to improve generalization and stabilize training.

---

## 🧠 Model Architecture

- Transfer Learning based CNN backbone  
- Custom Fully Connected Classification Head  
- Dropout Regularization  
- Softmax Output Layer  

---

## 🔬 Experimental Pipeline

Data Loading  
→ Preprocessing  
→ Augmentation  
→ Apply Imbalance Strategy  
→ Model Training  
→ Validation  
→ Metric Evaluation  
→ Strategy Comparison  

---

## 📊 Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- **Macro F1 Score (Primary Metric)**  
- **Confusion Matrix**

Main research focus: **Minority class recall improvement and Macro-F1 comparison**.

---

## 📁 Repository Structure

BUSI_Imbalance_Pipeline/  
│  
├── data/  
├── models/  
├── training/  
├── utils/  
├── experiments/  
├── train.py  
├── requirements.txt  
└── README.md  

---

## 🛠️ Tech Stack

- Python  
- PyTorch / TensorFlow  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 🚀 How to Run

### 1. Clone Repository

git clone https://github.com/Anuja0412Gupta/BUSI_Imbalance_Pipeline.git  
cd BUSI_Imbalance_Pipeline  

### 2. Install Dependencies

pip install -r requirements.txt  

### 3. Prepare Dataset

Download the BUSI dataset and update the dataset path inside the training configuration or script.

### 4. Run Training

python train.py --method focal  

### Available Methods

- baseline  
- augmentation  
- weighted_sampling  
- focal  
- smote  
- mixup  

---

## 📈 Results & Analysis

The repository provides:

- Performance comparison tables  
- Confusion matrix visualizations  
- Minority class recall improvements  
- Macro-F1 comparison plots  
- Training stability observations  

---

## 🔮 Future Work

- Vision Transformer based classification  
- Ensemble learning strategies  
- Grad-CAM explainability for medical interpretation  
- Hyperparameter optimization  
- Cross-dataset generalization experiments  

---

## 👩‍💻 Author

**Anuja Gupta**  
B.Tech Computer Science  
Interests: Deep Learning, Medical Imaging, AI Research  

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.
