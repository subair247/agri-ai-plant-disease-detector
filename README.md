# Plant Disease Classification using CNN 🌿🤖

A deep learning project built with **PyTorch** to detect and classify plant leaf diseases from images early, helping farmers protect crop yields using artificial intelligence[cite: 1, 2].

## 🚀 Overview
Early detection of plant diseases is critical in modern smart agriculture. This project implements a custom Convolutional Neural Network (CNN) from scratch using Python and PyTorch[cite: 1, 2] to accurately classify tomato leaf conditions across multiple categories[cite: 1].

## 📊 Dataset Structure
The dataset consists of real leaf photographs divided into the following categories mapped to standardized integer labels[cite: 1, 2]:
* **0**: Early Blight[cite: 1, 2]
* **1**: Healthy[cite: 1, 2]
* **2**: Late Blight[cite: 1, 2]
* **3**: Leaf Mold[cite: 1, 2]
* **4**: Septoria Leaf Spot[cite: 1, 2]
* **5**: Yellow Curl Virus[cite: 1, 2]

## 🛠️ Technical Stack
* **Language:** Python[cite: 4, 5]
* **Deep Learning Framework:** PyTorch, TorchVision[cite: 4, 5]
* **Data Manipulation & Analysis:** Pandas, NumPy[cite: 4, 5]
* **Metrics & Evaluation:** Scikit-Learn (Confusion Matrix, Accuracy Score)[cite: 5]
* **Image Processing:** Pillow (PIL)[cite: 4, 5]

## 🏗️ Project Architecture & Pipeline
1. **Exploratory Data Analysis:** Gathered image paths and organized class distributions into Pandas DataFrames[cite: 1, 2].
2. **Label Encoding:** Mapped categorical folder names to sequential integer labels[cite: 1, 2].
3. **Data Preprocessing & Loading:** Built custom PyTorch `Dataset` and `DataLoader` pipelines with dynamic image resizing (`64x64`) and an 80/20 train-validation split[cite: 2].
4. **CNN Architecture:** Designed a custom multi-layer Convolutional Neural Network featuring Convolutional layers, Batch Normalization, ReLU activations, Max-Pooling, Dropout regularization, and Fully Connected classification layers[cite: 2].
5. **Model Training:** Optimized using Cross-Entropy Loss and the Adam optimizer over multiple epochs[cite: 2].
6. **Evaluation:** Assessed model generalization using validation accuracy and Confusion Matrix metrics[cite: 2].

## ⚙️ Installation & Usage
1. Clone the repository:
   ```bash
   git clone (https://github.com/your-username/plant-disease-classification-cnn.git)
   cd plant-disease-classification-cnn
