# Abnormality Detection in Musculoskeletal Radiographs

This project focuses on the detection of abnormalities in musculoskeletal radiographs using a Convolutional Neural Network (CNN) architecture. The dataset used is the MURA dataset, which contains labeled X-ray images for various body parts, including the forearm and humerus. The goal is to classify images into normal and abnormal categories.

## Project Overview

- **Objective**: Develop a deep learning model to accurately classify X-ray images of forearm and humerus radiographs into normal and abnormal classes.
- **Dataset**: MURA v1.1, containing X-ray images annotated as positive (abnormal) and negative (normal).
- **Frameworks**: TensorFlow and Keras for building and training the CNN model.

## Key Features

- **Data Preprocessing**: 
  - Images are resized and normalized to enhance training effectiveness.
  - Data augmentation techniques (e.g., rotation, horizontal flip) are applied to the training set to improve model robustness.

- **Model Architecture**:
  - Custom CNN architecture designed with several convolutional layers, batch normalization, and max pooling layers.
  - Utilization of **DenseNet169** as a baseline model for feature extraction, combined with custom layers to enhance classification performance.

- **Training Process**:
  - The model is trained using a binary cross-entropy loss function with options for focal loss to handle class imbalance.
  - Class weights are calculated to ensure balanced training across normal and abnormal samples.
  - Early stopping and learning rate reduction callbacks are implemented to optimize training efficiency.

- **Validation and Testing**:
  - A validation set is created to monitor model performance during training.
  - Testing is conducted on a separate test set to evaluate model generalization.

## Results

The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. Confusion matrices are generated to analyze the classification results further. The implementation aims to achieve high sensitivity and specificity in detecting abnormalities in musculoskeletal radiographs.
