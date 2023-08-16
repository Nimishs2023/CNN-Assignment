# Melanoma Detection using Custom CNN

## Problem Statement
In this project, we build a custom convolutional neural network (CNN) model to accurately detect melanoma, a type of deadly skin cancer. The goal is to provide a solution that can evaluate images and alert dermatologists about the presence of melanoma, thereby reducing the manual effort needed in diagnosis.

## Dataset
The dataset consists of 2357 images of malignant and benign oncological diseases from the International Skin Imaging Collaboration (ISIC). The images are categorized into nine classes, including melanoma, nevus, squamous cell carcinoma, and more.

## Project Pipeline
1. **Data Reading & Understanding**: Load and preprocess the dataset, defining paths for train and test images.

2. **Dataset Creation**: Create train and validation datasets, resizing images to 180x180 pixels.

3. **Dataset Visualization**: Visualize instances of all nine classes present in the dataset.

4. **Model Building & Training (First Iteration)**: Build a CNN model to detect the nine classes, using appropriate optimization and loss functions. Train the model for around 20 epochs and analyze results for overfitting or underfitting.

5. **Data Augmentation & Model Building (Second Iteration)**: Apply data augmentation strategies to address overfitting/underfitting. Build and train the model again with augmented data.

6. **Class Distribution Analysis**: Examine class distribution in the training dataset, identify the classes with the least and most samples.

7. **Class Imbalance Handling**: Rectify class imbalances using the Augmentor library to generate augmented samples.

8. **Model Building & Training (Third Iteration)**: Rebuild the model on the rectified class imbalance data, train for around 30 epochs, and analyze results.

## Technologies Used
- Python
- TensorFlow
- Augmentor (for data augmentation)

## Conclusions
1. The initial model showed evidence of overfitting, as the training accuracy was higher than validation accuracy.
2. Data augmentation helped mitigate overfitting and improved the model's performance on unseen data.
3. Class distribution analysis revealed imbalanced classes, with melanoma having fewer samples.
4. Augmentation was applied to address class imbalances, but the model's test accuracy after handling imbalance was approximately 0.161.
5. While the test accuracy improved, the overall model performance may still need further improvement.
6. It's recommended to consider additional evaluation metrics such as precision, recall, and F1-score, especially in the context of imbalanced datasets.
7. Further analysis and fine-tuning of the model might be necessary to achieve better results on the task of melanoma detection.

## Acknowledgements
- The dataset used in this project is provided by the International Skin Imaging Collaboration (ISIC).
- This project was completed as part of the assignment for [Course Name/Institution].
