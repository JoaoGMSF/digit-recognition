# Handwritten Digit Recognition

This project performs handwritten digit recognition using **OpenCV** and the **k-Nearest Neighbors (k-NN)** algorithm.

## Overview

The goal of this project is to:

1. Process an image containing multiple handwritten digits.
2. Split the image into smaller cells representing each digit.
3. Train a machine learning model to recognize the digits using k-NN.
4. Evaluate the model's accuracy with a test dataset.

## Project Structure

The code is organized as follows:

- **Data Preparation**: The `digits.png` image is loaded and converted to grayscale. The image is then divided into 20x20 pixel cells, each representing individual digits.
  
- **Model Training**: The digits are split into two sets, one for training (70%) and one for testing (30%). We use the k-NN algorithm with k=3 to train the model.

- **Evaluation**: The accuracy of the model is calculated by comparing the k-NN results with the actual labels from the test set.

## Requirements

- **Python 3.x**
- **OpenCV**: Used to process images and build the model.

Install the required packages with the following command:

```bash
pip install opencv-python numpy