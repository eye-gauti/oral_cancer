# Oral Cancer Detection using Deep Learning

## Overview

This project focuses on the classification of oral cancer images using Convolutional Neural Networks (CNNs). Multiple deep learning architectures were explored and compared to identify the most effective model for binary classification of oral cancer conditions from image data.

The project evaluates the performance of:

* VGG16
* LeNet
* MobileNetV3

Among all tested architectures, **VGG16 achieved the best overall performance**, providing the highest validation accuracy and the most stable learning behavior.

---

## Dataset

The dataset used in this project consisted of approximately:

* **1000 total images**

  * 500 cancerous images
  * 500 non-cancerous images

Due to the relatively small dataset size, transfer learning and careful preprocessing techniques were important to improve model generalization.

> Note: The dataset is not included in this repository because of storage limitations and usage restrictions.

---

## Models Evaluated

| Model       | Training Accuracy | Validation Accuracy | Loss   |
| ----------- | ----------------- | ------------------- | ------ |
| VGG16       | 94.45%            | 91.68%              | 18.28% |
| LeNet       | 92.27%            | 78.67%              | 60.53% |
| MobileNetV3 | 72.15%            | 53.16%              | 68.68% |

### Best Performing Model: VGG16

VGG16 demonstrated the strongest classification capability among all tested architectures. Its higher validation accuracy indicates better feature extraction and improved generalization compared to LeNet and MobileNetV3 on this dataset.

---

## Project Structure

```text
oral-cancer-detection/
│
├── data/               # Dataset references and samples
├── models/             # Trained model weights
├── notebooks/          # Training and experimentation notebooks
├── results/            # Graphs, outputs, and evaluation results
├── requirements.txt
└── README.md
```

---

## Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Jupyter Notebook

---

## Features

* CNN-based oral cancer classification
* Comparative analysis of multiple architectures
* Transfer learning using VGG16
* Training and validation performance visualization
* Model evaluation and benchmarking

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/oral-cancer-detection.git
cd oral-cancer-detection
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

Run the notebooks from the `notebooks/` directory.

---

## Results

The experimental results show that transfer learning significantly improved performance on a limited medical imaging dataset.

Key observations:

* VGG16 achieved the best validation accuracy.
* LeNet performed reasonably well but showed weaker generalization.
* MobileNetV3 underperformed on this dataset, likely due to limited training data and feature complexity.

---

## Future Improvements

Several enhancements can further improve the system:

* Implementing deeper architectures such as:

  * ResNet
  * EfficientNet
  * DenseNet
* Increasing dataset diversity and size
* Collecting data from multiple medical sources
* Applying advanced augmentation techniques
* Hyperparameter optimization
* Building a real-time Streamlit web application
* Deploying lightweight models on edge devices and mobile platforms
* Integrating explainable AI techniques such as Grad-CAM for medical interpretability

---

## Applications

This project can contribute toward:

* Early oral cancer screening
* AI-assisted medical diagnosis
* Low-cost healthcare support systems
* Portable diagnostic solutions for rural healthcare environments

---

## Authors

Developed as part of an academic deep learning research project on medical image classification.

---

## License

This project is intended for educational and research purposes only.
