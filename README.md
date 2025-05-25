
# Wildlife Image Classification: Custom CNN vs MobileNetV2

This project focuses on classifying African wildlife images using deep learning techniques. It compares the performance of a custom Convolutional Neural Network (CNN) with a transfer learning approach using MobileNetV2.

## 📁 Dataset
The dataset consists of labeled images of African wildlife. It was split into training, validation, and test sets using the `splitfolders` library in the following ratio:
- 70% Training
- 20% Validation
- 10% Testing

## 🛠️ Model Architectures

### 🔹 Custom CNN
- 4 Convolutional layers with ReLU activation
- MaxPooling and Dropout for regularization
- Flatten + Dense layers for classification
- Trained from scratch

### 🔹 MobileNetV2
- Pretrained model used for feature extraction
- GlobalAveragePooling + Dense layers on top
- Fine-tuned for the dataset

## 🧪 Evaluation Metrics
- Confusion Matrix
- Classification Report

## 🔍 Key Findings
- MobileNetV2 significantly outperformed the custom CNN in terms of accuracy and generalization.
- Transfer learning enables faster convergence and better feature extraction, especially when the dataset is limited.

## 🚀 Libraries & Tools
- TensorFlow / Keras
- splitfolders
- Matplotlib / Seaborn
- Scikit-learn

## 📌 How to Run
1. Install required libraries:
```bash
pip install tensorflow split-folders
```
2. Run the notebook step-by-step in a Jupyter environment or on [Kaggle](https://www.kaggle.com/).
3. Ensure dataset is placed in the correct path (update `base_dir` if needed).


