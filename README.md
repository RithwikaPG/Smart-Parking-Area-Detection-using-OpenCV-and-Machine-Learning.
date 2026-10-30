# Smart-Parking-Area-Detection-using-OpenCV-and-Machine-Learning.
Developed a computer vision and machine learning-based parking space detection system using OpenCV and K-Nearest Neighbors (KNN) to classify parking spaces as empty or occupied.

## Project Overview

This project focuses on detecting whether a parking space is **EMPTY** or **OCCUPIED** using computer vision and machine learning techniques.

The system uses image processing techniques from OpenCV to prepare parking images and a K-Nearest Neighbors (KNN) algorithm to classify the parking space.

## Objectives

- Identify empty and occupied parking spaces from images.
- Apply image preprocessing techniques using OpenCV.
- Train a machine learning model for parking space classification.
- Evaluate the model using training and testing datasets.

## Technologies Used

- **Programming Language:** Python
- **Computer Vision:** OpenCV
- **Machine Learning:** Scikit-learn
- **Numerical Processing:** NumPy
- **Visualization:** Matplotlib
- **Dataset Download:** KaggleHub
- **Platform:** Google Colab

## Dataset

The project uses the Parking Dataset available on Kaggle.

**Dataset Link:** https://www.kaggle.com/datasets/rizwanrizwannazir/parking

| Category | Number of Images |
|---|---:|
| Empty Parking Spaces | 908 |
| Occupied Parking Spaces | 818 |
| **Total** | **1,726** |

## Methodology

### 1. Dataset Collection
Downloaded the parking dataset using the KaggleHub library. The dataset contains two categories: empty and occupied parking spaces.

### 2. Image Processing Using OpenCV
Applied the following image processing techniques:

- BGR to Grayscale Conversion
- Gaussian Blurring
- Canny Edge Detection
- Image Thresholding
- Contour Detection

### 3. Image Preprocessing
- Loaded all parking images.
- Resized images to 64 × 64 pixels.
- Converted images into grayscale.
- Flattened each image into a feature vector containing 4,096 values.
- Assigned numerical labels:
  - 0 – Empty
  - 1 – Occupied

### 4. Model Training
Used the K-Nearest Neighbors (KNN) classification algorithm with K = 5.

The dataset was divided into:
- 80% Training Data
- 20% Testing Data

### 5. Prediction
The trained model predicts whether a given parking space image is empty or occupied.

## Model Performance

The KNN classifier achieved approximately **70.23% accuracy** on the test dataset.

## Installation and Execution

Install the required libraries:

```bash
pip install kagglehub opencv-python numpy matplotlib scikit-learn
```

### Run Using Google Colab

1. Open the project notebook in Google Colab.
2. Run the cells sequentially.
3. The dataset will be downloaded using KaggleHub.
4. Execute the image preprocessing and model training steps.
5. Test the model using a parking space image.

## Future Improvements

- Improve classification accuracy using advanced machine learning algorithms.
- Implement CNN-based image classification.
- Integrate a live camera for real-time parking space detection.
- Extend the system to identify multiple parking spaces.
- Develop a dashboard to display parking space availability.

