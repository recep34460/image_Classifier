# SVM Image Classifier

This project is a straightforward machine learning pipeline for binary image classification. It uses a Support Vector Machine (SVM) algorithm to classify images into two categories: `empty` and `not_empty`.

## Features

* **Image Preprocessing:** Reads images from a specified directory, resizes them to 15x15 pixels for uniformity, and flattens them into 1D arrays suitable for machine learning models.
* **Hyperparameter Tuning:** Utilizes `GridSearchCV` to automatically test different combinations of `gamma` and `C` parameters, ensuring the SVM model achieves the highest possible accuracy.
* **Model Evaluation:** Splits the dataset into training and testing sets (80% train, 20% test) with stratification to evaluate the model's performance accurately.
* **Model Export:** Saves the best-performing model as a serialized `model.p` file using `pickle`, allowing it to be loaded and used for future predictions without retraining.

## Requirements and Installation

Make sure you have **Python 3.x** installed. You can install the required dependencies by running the following command:

```bash
pip install -r requirements.txt
