# Solar Panel Detection using YOLOv8

This repository contains the implementation of an object detection system designed to detect solar panels in satellite imagery. The project leverages Ultralytics YOLOv8 to train a model that accurately identifies solar panels from low-resolution satellite images.

## Overview

The primary goal of this project is to build and train an object detection model that focuses on solar panels. The steps carried out in this project include:

- **Data Exploration & Preprocessing:**  
  - Analyzing the dataset consisting of images (`image_chips_native`) and corresponding label files (`labels_native` and `labels_hd`).
  - Splitting the dataset into train, validation, and test sets while ensuring a one-to-one mapping between images and YOLO-format label files.
  - Filtering the labels to remove annotations that do not correspond to solar panels.

- **Environment Setup:**  
  - Creating a dedicated Conda environment using an `environment.yml` file.
  
- **Model Training:**  
  - Training a YOLOv8 model on the provided dataset.
  - Monitoring the training process, particularly ensuring that the validation loss converges over epochs.
  
- **Evaluation & Inference:**  
  - Evaluating model performance on the test set.
  - Visualizing predictions to verify that the model correctly detects solar panels.

## Environment Setup

It is recommended to use a dedicated Conda environment for this project. You can set up the environment using the provided `environment.yml` file. 
