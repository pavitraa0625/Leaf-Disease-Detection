# Leaf Disease Detection Using Deep Learning

## Overview

This project focuses on automated plant leaf disease classification using Deep Learning and Transfer Learning techniques. A MobileNetV2-based image classification model was developed to identify plant diseases from leaf images, helping support early disease detection and precision agriculture.

## Features

* Transfer Learning using MobileNetV2
* Image preprocessing and augmentation
* Train, Validation, and Test dataset splitting
* Fine-tuning for improved classification performance
* Model checkpointing and training log generation
* Performance evaluation on unseen test data

## Dataset

* Plant leaf image dataset
* 15 disease categories
* Images preprocessed and resized to 224 × 224 pixels

## Data Preprocessing

The following preprocessing techniques were applied:

* Image resizing (224 × 224)
* Normalization
* Data augmentation:

  * Rotation
  * Horizontal flipping
  * Zoom augmentation
  * Width and height shifting

## Model Architecture

### Base Model

* MobileNetV2 (Pre-trained on ImageNet)

### Classification Head

* Global Average Pooling Layer
* Dense Layer
* Dropout Layer
* Softmax Output Layer

## Training Strategy

### Feature Extraction Phase

* MobileNetV2 base layers frozen
* Custom classification head trained

### Fine-Tuning Phase

* Selected MobileNetV2 layers unfrozen
* Batch Normalization layers kept frozen
* Low learning rate used for stable convergence

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Google Colab
* Matplotlib

## Repository Contents

* Training Notebook
* Fine-Tuning Notebook
* Model Checkpoints
* Training Logs
* Experimental Results

## Applications

* Smart Agriculture
* Crop Health Monitoring
* Early Disease Detection
* Precision Farming

## Future Improvements

* Deploy as a web application
* Real-time disease detection
* Mobile application integration
* Support for additional crop species

## Author

**Pola Pavitra Kumari**

GitHub: https://github.com/pavitraa0625
