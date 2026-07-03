# Federated Machine Learning using CICIoV2024 for detection of intrusion detection from internet of vehicles
Federated Learning model implementation using a Convolutional Neural Network (CNN) trained and evaluated on the CICIoV2024 dataset for intrusion detection in in-vehicle networks.

https://ieeexplore.ieee.org/abstract/document/11563534

Proactive Threat Hunting and Anomaly Detection in Intelligent Green Transportation: A Federated Edge-AI Framework for In-Vehicle Consumer Networks

Overview

This project implements a Federated Learning model using a Convolutional Neural Network (CNN). The model is trained and tested on the CICIoV2024 dataset to detect intrusions in in-vehicle networks.

The main goal of this project is to build a privacy-preserving intrusion detection system for Internet of Vehicles (IoV) environments. In this system, data remains with each client, and only model updates are shared. This helps protect data privacy while maintaining good detection accuracy.

Objectives

The main objectives of this project are:

Develop a CNN-based model to detect attacks in IoV network data.

Use Federated Learning to train the model without sharing private client data.

Evaluate the model using accuracy, precision, recall, F1-score, confusion matrix, and AUC.

Test the model for both binary classification and multi-class classification.

Federated Learning Configuration

The Federated Learning setup follows the TensorFlow Federated (TFF) structure. The process works as follows:

Model Initialization: A global CNN model is created and sent to all clients.

Local Training: Each client trains the CNN model using its own private data.

Model Aggregation: The trained model updates from all clients are collected and combined on the central server.

Global Update: The updated global model is sent back to the clients.

Repeated Training: These steps are repeated for several rounds until the model performance becomes stable.

Dataset: CICIoV2024

The CICIoV2024 dataset is used for intrusion detection in in-vehicle networks. It contains labeled CAN-bus traffic data, including both normal traffic and attack traffic from different vehicle ECUs.

Key features of the dataset include:

Realistic IoV attack scenarios.

Preprocessed and balanced features.

Suitable for CNN-based intrusion detection models.

Suitable for Federated Learning experiments.

Evaluation Metrics

The model is evaluated using the following metrics:

Accuracy

Precision

Recall

F1-score

Confusion matrix

AUC curve

The project supports both binary classification and multi-class classification.
