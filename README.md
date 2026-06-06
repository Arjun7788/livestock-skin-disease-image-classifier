# livestock-skin-disease-image-classifier

## Project Overview
This project uses Convolutional Neural Networks (CNN) and Transfer Learning (MobileNetV2) to classify livestock skin diseases from image data. The objective is to assist in the early detection of skin diseases in animals through automated image classification.


## Dataset

The dataset contains images of livestock categorized into three classes:

* Healthy
* Lumpy Skin Disease
* Foot-and-Mouth Disease

### Dataset Statistics

| Dataset Split  | Images |
| -------------- | ------ |
| Training Set   | 2,269  |
| Validation Set | 485    |
| Test Set       | 505    |
| Total Images   | 3,259  |

### Class Distribution

#### Training Set

* Healthy: 903 images
* Lumpy Skin Disease: 844 images
* Foot-and-Mouth Disease: 522 images

#### Validation Set

* Healthy: 193 images
* Lumpy Skin Disease: 181 images
* Foot-and-Mouth Disease: 111 images

#### Test Set

* Healthy: 195 images
* Lumpy Skin Disease: 197 images
* Foot-and-Mouth Disease: 113 images

### Image Information

* Total Classes: 3
* Image Formats: JPG and PNG
* Input Image Size: 224 × 224 pixels
* Task Type: Multi-class Image Classification

Dataset Link:
[https://www.kaggle.com/datasets/devang03mgr/cattle-diseases-datasets/data](url)



## Project Structure

livestock-skin-disease-classifier/
│
├── notebooks/
│   └── Livestock_Skin_Disease_Classifier.ipynb
├── README.md
├── dataset_link.txt
└── figures/



## Methodology

1. Dataset Loading
2. Data Preprocessing
3. Data Augmentation
4. Custom CNN Model Development
5. CNN Training and Evaluation
6. Transfer Learning using MobileNetV2
7. Model Comparison



## Models Used

### Custom CNN
A Convolutional Neural Network built from scratch for image classification.

### MobileNetV2
A pre-trained MobileNetV2 model used for transfer learning.



## Results
The performance of both models was evaluated using:

- Accuracy
- Loss Curves
- Confusion Matrix
- Classification Metrics

MobileNetV2 achieved better generalization performance compared to the custom CNN model.


## Visualizations

The figures folder contains:

- CNN Accuracy Curve
- CNN Loss Curve
- CNN Confusion Matrix
- MobileNetV2 Accuracy Curve
- MobileNetV2 Loss Curve
- MobileNetV2 Confusion Matrix


  ## Requirements

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
