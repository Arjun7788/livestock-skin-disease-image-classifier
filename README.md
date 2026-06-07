# Livestock Skin Disease Image Classifier

## Project Overview

This project focuses on classifying livestock skin disease images using deep learning techniques. The objective is to automatically identify whether an animal is healthy or affected by a skin disease based on image data.

Three classes are considered:

* Healthy
* Lumpy Skin Disease
* Foot-and-Mouth Disease

Two models were implemented and compared:

1. Custom Convolutional Neural Network (CNN)
2. MobileNetV2 Transfer Learning Model

---

## Dataset Information

Dataset: Cattle Diseases Dataset

Dataset Link:
https://www.kaggle.com/datasets/devang03mgr/cattle-diseases-datasets

### Dataset Statistics

| Dataset Split  | Images |
| -------------- | ------ |
| Training Set   | 2269   |
| Validation Set | 485    |
| Test Set       | 505    |
| Total Images   | 3259   |

### Class Distribution

#### Training Set

* Healthy: 903
* Lumpy Skin Disease: 844
* Foot-and-Mouth Disease: 522

#### Validation Set

* Healthy: 193
* Lumpy Skin Disease: 181
* Foot-and-Mouth Disease: 111

#### Test Set

* Healthy: 195
* Lumpy Skin Disease: 197
* Foot-and-Mouth Disease: 113

### Image Information

* Image Formats: JPG and PNG
* Number of Classes: 3
* Input Image Size: 224 × 224
* Task Type: Multi-Class Image Classification

---

## Methodology

The project follows the following workflow:

1. Dataset Loading
2. Image Preprocessing
3. Image Resizing and Normalization
4. Data Augmentation
5. Custom CNN Development
6. CNN Training and Evaluation
7. Transfer Learning using MobileNetV2
8. Model Comparison

---

## Models Used

### Custom CNN

Architecture:

* Conv2D (32 filters)
* MaxPooling2D
* Conv2D (64 filters)
* MaxPooling2D
* Conv2D (128 filters)
* MaxPooling2D
* Flatten Layer
* Dense Layer (128 neurons)
* Dropout (0.5)
* Softmax Output Layer

### MobileNetV2

Architecture:

* MobileNetV2 (ImageNet Pretrained)
* Global Average Pooling Layer
* Dense Layer (128 neurons)
* Dropout (0.5)
* Softmax Output Layer

---

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

---

## Results

| Model       | Test Accuracy |
| ----------- | ------------- |
| Custom CNN  | 75.25%        |
| MobileNetV2 | 88.12%        |

MobileNetV2 achieved the highest performance and outperformed the custom CNN model by approximately 12.87 percentage points.

---

## Repository Structure

```text
livestock-skin-disease-classifier/
│
├── Livestock_Skin_Disease_Classifier.ipynb
├── README.md
├── dataset_link.txt
└── figures/
```

---

## Output Figures

The repository includes:

* CNN Accuracy Curve
* CNN Loss Curve
* CNN Confusion Matrix
* MobileNetV2 Accuracy Curve
* MobileNetV2 Loss Curve
* MobileNetV2 Confusion Matrix

---

## How to Run the Project

1. Open the notebook in Google Colab.
2. Mount Google Drive.
3. Upload or connect the dataset.
4. Update dataset paths if required.
5. Run all notebook cells sequentially.
6. Evaluate the generated results and figures.

---

## Author

Arjun Meghanandbhai Mod

M.Sc. Data Science

University of Europe For Applied Sciences 
