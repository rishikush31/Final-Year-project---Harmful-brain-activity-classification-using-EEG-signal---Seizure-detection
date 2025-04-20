# 🧠 Harmful Brain Activity Classification Using EEG Signals (Seizure Detection)

## 📍 Overview

This project focuses on the detection of epileptic seizures using EEG signals. By converting EEG signal data into images, we classify brain activity into seizure vs. non-seizure using deep learning models pre-trained on ImageNet. We benchmark multiple CNN architectures to identify the most effective one for this task.

## 📂 Dataset

The dataset is sourced from Kaggle: [Seizure Detection EEG Dataset](https://www.kaggle.com/datasets/)

- It contains EEG recordings from multiple individuals with seizure and non-seizure activity.
- Data is preprocessed and converted into spectrogram/image form to make it suitable for CNN-based classification.

## 🎯 Objective

To build an accurate and efficient model that can detect seizures from EEG signals using deep learning.

## 🧪 Models Tested

| Model              | Loss   | Accuracy | Precision | Recall | F1-Score |
|-------------------|--------|----------|-----------|--------|----------|
| **VGG16**         | 0.471  | 0.822    | 0.676     | 0.822  | 0.742    |
| **EfficientNetV2**| 1.825  | 0.704    | 0.710     | 0.704  | 0.707    |
| **ResNet152V2**   | 0.468  | 0.822    | 0.676     | 0.822  | 0.742    |
| **VGG19**         | 1.084  | 0.822    | 0.676     | 0.822  | 0.742    |

> ⚠️ Fill in the metrics after model evaluation.

## 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 🧠 Preprocessing

- EEG signals are converted into spectrogram images using STFT or other transformation methods.
- Normalization and resizing to 224x224 (or required input size).
- Augmentation (optional) to enhance generalization.

## 🛠️ Tools & Frameworks

- Python
- TensorFlow / Keras
- NumPy & Pandas
- OpenCV / Librosa (for image or audio preprocessing)
- Matplotlib & Seaborn (for visualizations)
