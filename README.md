# Project Readme

## Scientist Image Classification Project

### Overview

This project is aimed at classifying scientist images using machine learning techniques. It involves detecting faces and eyes in the images, extracting features from the images, and training a machine learning model to classify scientists based on their facial features.

### Table of Contents

1. [Project Description](#project-description)
2. [Dependencies](#dependencies)
3. [Usage](#usage)
4. [Data Collection](#data-collection)
5. [Data Preprocessing](#data-preprocessing)
6. [Feature Extraction](#feature-extraction)
7. [Model Training](#model-training)
8. [Model Evaluation](#model-evaluation)
9. [Model Deployment](#model-deployment)
10. [Conclusion](#conclusion)

### 1. Project Description<a name="project-description"></a>

The goal of this project is to classify scientist images into different categories. The project involves several steps, including data collection, data preprocessing, feature extraction, model training, and model evaluation. The main tasks in each step are as follows:

### 2. Dependencies<a name="dependencies"></a>

Before running the project, make sure you have the following dependencies installed:

- Python (3.7 or higher)
- OpenCV
- NumPy
- Matplotlib
- scikit-learn
- Flask (for server deployment)

You can install these dependencies using `pip install` if they are not already installed.

### 3. Usage<a name="usage"></a>

The project can be run by executing the provided Jupyter Notebook file (`scientist_image_classification.ipynb`). This notebook contains all the code required for data preprocessing, feature extraction, model training, and evaluation.

To classify a scientist image, follow these steps:

1. Load the image using OpenCV.
2. Preprocess the image, including converting it to grayscale.
3. Detect faces and eyes in the image using Haar cascades.
4. Extract features from the image.
5. Use a trained machine learning model to predict the scientist's category.

The Flask server can be used to deploy the trained model and make predictions through HTTP requests.

### 4. Data Collection<a name="data-collection"></a>

The project uses a dataset of scientist images. The dataset should be organized in folders, with each folder representing a different scientist. The images should be named appropriately.

### 5. Data Preprocessing<a name="data-preprocessing"></a>

Data preprocessing includes loading the images, converting them to grayscale, and cropping the images to focus on the scientist's face. The preprocessed images are then saved to a new folder.

### 6. Feature Extraction<a name="feature-extraction"></a>

Feature extraction is performed using the Wavelet Transform. It extracts features from both the raw and preprocessed images. The extracted features are then combined into a feature vector.

### 7. Model Training<a name="model-training"></a>

The project uses a Support Vector Machine (SVM) with an RBF kernel to train the classification model. The model is trained on the extracted features from the scientist images.

### 8. Model Evaluation<a name="model-evaluation"></a>

The trained model's performance is evaluated using classification metrics such as accuracy, precision, recall, and F1-score. The confusion matrix is also visualized.

### 9. Model Deployment<a name="model-deployment"></a>

The trained model can be deployed as a Flask web service to make predictions via HTTP requests. The Flask server code is not provided in the Jupyter Notebook but can be found in the Flask server script.

### 10. Conclusion<a name="conclusion"></a>

This project demonstrates the process of classifying scientist images using machine learning techniques. It involves data collection, preprocessing, feature extraction, model training, and evaluation. The trained model can be deployed as a web service to make predictions on new scientist images.

Please make sure to follow the instructions in the Jupyter Notebook and Flask server script to run the project successfully.

For any questions or issues, feel free to contact the project owner.

**Note:** Make sure to save the trained model and class dictionary for future use and deployment.