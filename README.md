# DL_Mini_Project

# Human Activity Recognition with Deep Learning

## Problem Statement

Human Activity Recognition (HAR) is a key problem in fields like healthcare, smart homes, and fitness monitoring. The objective of this project is to detect and classify physical activities performed by individuals using sensor data collected from smartphones.

This project explores different deep learning models — including CNN and LSTM — to both detect anomalies (binary classification) and perform full activity recognition (multi-class classification).

---

## Models Trained

### 1. **Binary Class CNN for Anomaly Detection**
- Purpose: Detect whether an activity is "normal" (e.g., walking) or an "anomaly" (e.g., not walking).
- Model: 1D CNN using a sigmoid output and binary crossentropy.
- Output: 0 = Normal, 1 = Anomaly

### 2. **Multi-Class CNN**
- Purpose: Classify one of the 6 activities performed.
- Model: 1D Convolutional Neural Network using softmax activation.
- Output Classes:
  - 1 = Walking
  - 2 = Walking Upstairs
  - 3 = Walking Downstairs
  - 4 = Sitting
  - 5 = Standing
  - 6 = Laying

### 3. **Multi-Class LSTM**
- Purpose: Same as above, but leverages the temporal sequence of data more deeply.
- Model: Stacked LSTM layers with softmax output.
- Advantage: Learns temporal dependencies in sensor readings across time steps.

---

## 🔍 Dataset

We use the [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones), which includes accelerometer and gyroscope data collected from 30 participants performing various physical activities.

-  Features: 561 engineered features per sample
-  Classes: 6 activity labels
-  Data Shape: 
  - Training: 7352 samples
  - Testing: 2947 samples

---

##  Summary

This project demonstrates the application of deep learning on sensor data to recognize human activities. It compares three different architectures and provides insights on which models perform better for which tasks.

By accurately recognizing activities, such models can be deployed in fitness apps, smart environments, and medical alert systems.

