# pothole-Detection-ml
Project Overview

This project implements a pothole detection system using machine learning techniques. Road images are classified into two categories — Normal Road and Pothole — using Support Vector Machine (SVM) and Random Forest Classifier.

The system performs image preprocessing, feature extraction, model training, evaluation, and prediction on custom test images.

Objectives

Detect potholes from road images

Compare performance of SVM and Random Forest

Build a simple and effective ML-based solution for road safety analysis

Allow testing on user-provided images

Models Used

Support Vector Machine (SVM) with RBF kernel

Random Forest Classifier

Both models are trained and evaluated on the same dataset to compare accuracy and classification performance.

Dataset Description

The dataset contains road images organized into two folders:

normal → images without potholes

potholes → images containing potholes

Folder Structure
archive (1)/
 ├── normal/
 └── potholes/


Note:
Google Drive mounting was not possible due to authentication issues in Google Colab.
Hence, the dataset is uploaded manually as a ZIP file during runtime using Colab’s file upload feature.

Technologies & Libraries Used

Python

OpenCV

NumPy

Scikit-learn

Matplotlib

Seaborn

Google Colab

Methodology
1. Dataset Upload & Extraction

Dataset ZIP (images.zip) is uploaded manually using files.upload()

Files are extracted inside the Colab environment

2. Image Preprocessing

Resize images to 128 × 128

Convert images to grayscale

Flatten image matrices into feature vectors

3. Label Encoding

0 → Normal Road

1 → Pothole

4. Train-Test Split

80% training data

20% testing data

Stratified split to maintain class balance

Model Evaluation
Metrics Used

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Results

Random Forest achieved better performance compared to SVM

Confusion matrices are visualized using heatmaps for both models

(Exact accuracy values depend on dataset size and quality.)


Testing on Custom Image

The project allows testing on a user-provided image:

Image is preprocessed in the same way as training data

The trained model predicts whether the image contains a pothole

Output Example
Prediction: Pothole or Normal

Limitations

1.Uses traditional ML models instead of deep learning

2.Performance depends on image quality and dataset size

3.Real-time detection not implemented

Future Enhancements

1.Use CNN / Deep Learning for improved accuracy

2.Real-time pothole detection using video input

3.GPS-based pothole mapping

4.Mobile or web-based deployment
