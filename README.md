# Agri AI Plant Disease Detector 🌿🤖

A robust deep learning pipeline built with **PyTorch** designed for early-stage crop disease detection and classification using Convolutional Neural Networks (CNNs). This project aims to empower smart agriculture systems by accurately identifying plant health conditions from leaf imagery to protect crop yields[cite: 1, 2].

---

## 🌟 Key Features
* **Custom CNN Architecture:** Engineered from scratch using PyTorch with customized convolutional blocks, batch normalization, max-pooling, and dropout regularization[cite: 2].
* **End-to-End ML Pipeline:** Covers automated data loading, exploratory data analysis, label encoding, stratified train-validation splitting, model training, and performance evaluation[cite: 1, 2].
* **Rigorous Evaluation:** Utilizes multi-class metrics including validation accuracy, confusion matrix analysis, and sample-level prediction verification[cite: 2].

---

## 📂 Dataset & Classes
The model is trained to classify tomato leaf photographs into 6 distinct categories mapped to standardized integer labels[cite: 1, 2]:

| Class Name | Assigned Label | Description / Status |
| :--- | :---: | :--- |
| **Early_Blight** | `0` | Fungal infection affecting foliage[cite: 1, 2] |
| **Healthy** | `1` | Normal, disease-free leaf structure[cite: 1, 2] |
| **Late_Blight** | `2` | Aggressive pathogen affecting crops[cite: 1, 2] |
| **Leaf_Mold** | `3` | Common greenhouse leaf condition[cite: 1, 2] |
| **Septoria_Leaf_Spot** | `4` | Spotting disorder on plant leaves[cite: 1, 2] |
| **Yellow_Curl_Virus** | `5` | Viral infection causing leaf distortion[cite: 1, 2] |

---

## 🛠️ Tech Stack & Libraries
* **Programming Language:** Python[cite: 4, 5]
* **Deep Learning Framework:** PyTorch, TorchVision[cite: 4, 5]
* **Data Processing & Analysis:** Pandas, NumPy[cite: 4, 5]
* **Computer Vision / Image Handling:** Pillow (PIL)[cite: 4, 5]
* **Evaluation Metrics:** Scikit-Learn (Accuracy Score, Confusion Matrix)[cite: 5]

---

## 🏗️ Architectural Workflow

1. **Exploratory Data Analysis (EDA):** Gathered and indexed image file paths, structuring them into Pandas DataFrames to inspect class distributions and sample images[cite: 1, 2].
2. **Label Encoding:** Mapped alphabetical class folders to numeric label indices (`0` to `5`)[cite: 1, 2].
3. **Data Preprocessing & Dataloaders:** Created custom PyTorch `Dataset` classes incorporating image resizing (`64x64`), tensor conversion, and stratified 80/20 train-validation splitting[cite: 2].
4. **Model Architecture Design:** Built a modular CNN featuring sequential feature extraction layers followed by fully connected dense layers with dropout to prevent overfitting[cite: 2].
5. **Model Optimization:** Trained using Cross-Entropy Loss and the Adam optimizer over multiple epochs with live accuracy and loss tracking[cite: 2].
6. **Evaluation & Validation:** Generated confusion matrices and performed validation checks to verify generalization on unseen leaf structures[cite: 2].

---

## 🚀 Getting Started

### Prerequisites
Ensure you have Python installed along with pip. 

### Installation
1. Clone the repository:
   ```bash
   git clone (https://github.com/your-username/agri-ai-plant-disease-detector.git)
   cd agri-ai-plant-disease-detector
