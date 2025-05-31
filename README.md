# Computer Vision Project: Real Age Prediction

## Project Description

This project focuses on developing a Computer Vision model to predict the real (chronological) age of individuals from facial images. The dataset consists of a collection of facial photographs and corresponding age labels.

## Analysis Goal

The goal of the exploratory data analysis (EDA) conducted in the accompanying Jupyter Notebook was to gain a comprehensive understanding of the dataset's characteristics. This included examining the dataset size, exploring the distribution of ages, and visualizing sample images across different age ranges. The insights gained from this EDA will inform the subsequent modeling stage and help in identifying potential challenges and strategies for training an effective age prediction model. Additionally, the project reviews the results of a pre-trained model to understand its performance on this task.

## Technologies Used

* **Python**
* **TensorFlow / Keras:** For building, training, and evaluating deep learning models, leveraging `ImageDataGenerator` for efficient large-scale image data handling.
* **OpenCV (cv2):** For image processing tasks (e.g., loading, resizing, normalization).
* **NumPy:** For numerical operations and array manipulation.
* **Pandas:** For handling and organizing tabular data (e.g., `labels.csv`).
* **Matplotlib / Seaborn:** For visualizing data distributions, model training progress, and evaluation results.
* **Jupyter Notebook:** The primary environment for conducting the analysis, experimentation, and presenting findings.

## Dataset

**Important Note on Data Availability:** Due to the large size of the image data (7.6k photos), the dataset itself is **not included** in this GitHub repository. 

## Analysis & Results

The `real_age_prediction.ipynb` notebook contains the complete code for:
* Exploratory Data Analysis (EDA) of the dataset (size, age distribution, sample visualizations).
* Data preprocessing, including preparing data for `ImageDataGenerator`.
* Building and compiling the deep learning model architecture.
* Training the model (though full execution requires the dataset).
* Evaluating model performance.
* Visualizing key findings, training curves, and analysis results.

All significant outputs, plots, and key findings from the original analysis are already displayed within the notebook cells in this repository.
