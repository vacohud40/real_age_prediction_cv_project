# Real Age Prediction from Facial Images

## Project Overview

This project develops a **Computer Vision model** to predict the real age of individuals from facial images. The primary objective was to build a robust model capable of estimating age accurately, complemented by an **Exploratory Data Analysis (EDA)** to understand the dataset's characteristics and inform modeling strategies.

## Key Features & Technologies

* **Computer Vision (CV)**: Core focus on image-based age prediction.
* **Deep Learning**: Utilizes **TensorFlow/Keras** for model development.
* **Transfer Learning**: Employs **ResNet50** as a pre-trained backbone.
* **Data Handling**: Efficiently manages large image datasets using **`ImageDataGenerator`**.
* **Programming Languages**: Developed primarily in **Python**.
* **Libraries**: Leverages **Pandas**, **NumPy**, and **Matplotlib** for data manipulation, numerical operations, and visualization.

## Dataset

The dataset consists of approximately **7,600 facial photographs** located in `/datasets/faces/final_files/`, with corresponding age labels in `labels.csv` (`file_name`, `real_age`). Due to its size, images are loaded using `ImageDataGenerator` to optimize computational resources.

## Exploratory Data Analysis (EDA) Summary

The EDA revealed that the dataset's **age distribution is imbalanced**, with a higher concentration of samples in the 20-30 age range. Visual inspection highlighted **significant variability** in image quality, lighting, pose, and facial expressions, posing challenges for model generalization.

## Model Architecture

The model utilizes a **ResNet50** pre-trained on ImageNet as a convolutional backbone, followed by a GlobalAveragePooling2D layer and dense layers for regression-based age prediction. It's compiled with Mean Squared Error (MSE) loss and Mean Absolute Error (MAE) as a metric, optimized with the Adam optimizer.

## Results

After 20 epochs of training, the model achieved a **final validation MAE of approximately 7.65 years**. While training loss generally decreased, fluctuations in validation metrics suggested potential areas for further optimization to improve generalization.

## How to Run

The model can be trained on a **GPU platform**. A consolidated script, including all necessary functions and initialization, can be generated and executed. Ensure the dataset (`/datasets/faces/final_files/` and `labels.csv`) is accessible in the specified path.
