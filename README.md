# Multi-Class Food Image Classification Using ResNet-18 with Optuna Optimization

## Overview

This project focuses on detecting and classifying multiple food items present in a single plate image.
A deep learning model based on **ResNet-18** is trained on a food image dataset containing 20 food categories.

To improve model performance, **Optuna** is used for automated hyperparameter optimization.
During testing, a **sliding window approach** is used to scan the plate image and identify food items.

---

## Dataset

The model is trained on the **Food Image Classification Challenge Dataset** from Kaggle.

Dataset details:

* Total images: **6003**
* Number of classes: **20 food categories**
* Each class contains approximately **300 images**

Examples of food categories include:

* biryani
* dosa
* idli
* samosa
* gulab jamun
* fried rice
* chapati

---

## Project Objectives

The main objectives of this project are:

* Train a deep learning model to classify food images.
* Optimize hyperparameters using **Optuna**.
* Detect multiple food items in a single plate image.
* Visualize detected food items using circular annotations.

---

## Model Architecture

The project uses **ResNet-18**, a convolutional neural network designed for image classification.

Key features:

* Residual learning using skip connections
* Efficient deep feature extraction
* Good performance on image classification tasks

The final layer of ResNet-18 is modified to classify **20 food categories**.

---

## Hyperparameter Optimization

The **Optuna framework** is used to automatically tune model hyperparameters such as:

* Learning rate
* Batch size
* Optimizer type
* Weight decay

Optuna performs multiple trials and selects the best configuration based on validation accuracy.

---

## Methodology

The workflow of the project is as follows:

1. **Dataset Preprocessing**

   * Resize images
   * Normalize pixel values
   * Apply data augmentation

2. **Model Training**

   * Train ResNet-18 on single food item images
   * Use Optuna for hyperparameter tuning

3. **Model Evaluation**

   * Evaluate model performance on validation dataset
   * Measure classification accuracy

4. **Sliding Window Detection**

   * Apply sliding window across plate image
   * Classify each region using trained model
   * Filter detections based on confidence score

5. **Visualization**

   * Draw circles around detected food items
   * Display predicted class labels

---

## Technologies Used

* Python
* PyTorch
* OpenCV
* Matplotlib
* NumPy
* Optuna

---

## Results

The trained model successfully classifies food images from 20 categories and detects multiple food items in a plate image using a sliding window approach.

The output visualization highlights detected food items using circular markers along with predicted labels.

---

## Future Work

Possible improvements for this project include:

* Implementing more advanced object detection methods
* Using larger food image datasets
* Improving detection accuracy for overlapping food items
* Deploying the model as a web or mobile application

---

## Author

**Poojitha Valluri**

Project: Multi-Class Food Image Classification Using ResNet-18 with Optuna-Based Hyperparameter Optimization
