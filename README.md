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

| Model                          | Architecture Preview | Accuracy | Precision | Recall | F1-Score |
|-------------------------------|----------------------|----------|-----------|--------|----------|
| **VGG16**                     | ![VGG16](https://raw.githubusercontent.com/rajpurkar/deepslate/main/media/vgg16.png) |          |           |        |          |
| **EfficientNet (ImageNet)**   | ![EfficientNet](https://raw.githubusercontent.com/qubvel/efficientnet/master/images/efficientnet.png) |          |           |        |          |
| **VGG19 (ImageNet)**          | ![VGG19](https://miro.medium.com/v2/resize:fit:1400/1*VUe0bKnzJ3AGni3x5K3aYA.png) |          |           |        |          |
| **ResNet (ImageNet)**         | ![ResNet](https://neurohive.io/wp-content/uploads/2018/11/resnet-architecture.png) |          |           |        |          |

> ⚠️ Replace the metrics above after training and evaluation.

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
- Matplotlib & Seaborn (for visualizations)
