# Brain Tumor Detection Using Deep Learning

## Overview

Brain Tumor Detection is a deep learning-based image classification system designed to automatically identify and classify brain tumors from MRI scans. The project leverages Convolutional Neural Networks (CNNs) and Transfer Learning techniques to achieve accurate tumor classification.

The system categorizes MRI images into four classes:

* Glioma Tumor
* Meningioma Tumor
* Pituitary Tumor
* No Tumor

The project explores multiple deep learning architectures, including a custom CNN, VGG16, and EfficientNetB0, to compare performance and improve classification accuracy.

---

## Features

* Automated MRI image classification
* Multi-class tumor detection
* Image preprocessing and normalization
* Data augmentation for improved generalization
* Custom CNN implementation
* Transfer Learning using VGG16
* Transfer Learning using EfficientNetB0
* Early stopping and learning rate scheduling
* Confusion matrix visualization
* Classification report generation
* Model saving and loading support

---

## Dataset

The dataset consists of brain MRI images organized into four categories:

```text
Training/
├── glioma
├── meningioma
├── pituitary
└── notumor

Testing/
├── glioma
├── meningioma
├── pituitary
└── notumor
```

---

## Data Preprocessing

The following preprocessing steps were applied:

* Image resizing to 150 × 150 pixels
* Pixel value normalization
* Data augmentation

  * Rotation
  * Zoom
  * Width shift
  * Height shift
  * Horizontal flipping

---

## Model Architectures

### Custom CNN

* Conv2D Layers
* MaxPooling Layers
* Dense Layers
* Softmax Output Layer

### VGG16 Transfer Learning

* Pretrained ImageNet weights
* Feature extraction
* Fine-tuning of upper layers
* Dropout regularization

### EfficientNetB0 Transfer Learning

* Efficient feature extraction
* Transfer learning approach
* Learning rate scheduling
* Early stopping mechanism

---

## Performance

The optimized transfer learning model achieved:

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 94.84% |
| Precision | 95%    |
| Recall    | 95%    |
| F1-Score  | 95%    |

---

## Technologies Used

* Python
* TensorFlow
* Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/brain-tumor-detection.git
cd brain-tumor-detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Train the model:

```bash
python train.py
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

Load a saved model:

```python
import tensorflow as tf

model = tf.keras.models.load_model("brain_tumor_model.keras")
```

---

## Project Workflow

1. Data Collection
2. Data Preprocessing
3. Data Augmentation
4. Model Training
5. Model Evaluation
6. Performance Analysis
7. Prediction on New MRI Images

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Future Enhancements

* Web Application Deployment
* Explainable AI (Grad-CAM)
* Real-Time Prediction Interface
* Model Optimization
* Medical Decision Support Integration

---

## License

This project is intended for educational and research purposes.
