# Face Mask Detection through Webcam

![evaluation](https://user-images.githubusercontent.com/41834661/115959474-fc4bcb80-a529-11eb-888e-de6b95d0dd13.png)

![Screenshot_1](https://user-images.githubusercontent.com/41834661/115959414-c3abf200-a529-11eb-97dd-b7360f06272f.png)

This project aims to implement real-time face mask detection through a webcam feed using deep learning techniques. With the ongoing global pandemic, ensuring proper face mask usage has become crucial in controlling the spread of infectious diseases. This system provides a convenient way to monitor whether individuals are wearing masks properly in real-time.

## Overview

The project consists of two main components:

1. **Model Training**: This involves training a deep learning model to detect whether a person is wearing a mask correctly or not. The model is trained on a dataset consisting of images of people with and without masks.

2. **Real-time Detection**: Once the model is trained, it is utilized to perform face mask detection on live webcam feeds. The system detects faces in the video stream and then determines whether each detected face is wearing a mask or not.

## Model Training

### Files:

- **Data Augmentation and Model Training.ipynb**: This Jupyter Notebook contains the detailed process of data augmentation and model training. It includes steps such as loading the dataset, preprocessing images, defining the model architecture, training the model, and evaluating its performance.

- **face_detector.zip**: This file contains a pre-trained face detector model, which is used to detect faces in the webcam feed during real-time detection.

- **mask-detector-model.model**: After training the model, it is saved to this file for later use in real-time detection.

- **requirements.txt**: This file lists all the dependencies required to run the model training script.

## Real-time Detection

### Files:

- **detect_mask_from_webcam.py**: This Python script is responsible for performing face mask detection on live webcam feeds. It utilizes the pre-trained face detector model to detect faces in the video stream and then uses the trained face mask detector model to determine whether each detected face is wearing a mask or not.

## Usage

To use the real-time face mask detection system:

1. Ensure all dependencies listed in `requirements.txt` are installed.
2. Run the `detect_mask_from_webcam.py` script.
3. The script will access your webcam and start detecting faces in real-time, overlaying the results on the video feed.
