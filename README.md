# Federated-Learning-with-CNN-using-CICIoV2024
Federated Learning model implementation using a Convolutional Neural Network (CNN) trained and evaluated on the CICIoV2024 dataset for intrusion detection in in-vehicle networks.

📘 Overview:

This repository presents an implementation of a Federated Learning (FL) framework integrated with a Convolutional Neural Network (CNN) model, trained and evaluated using the CICIoV2024 dataset. The project aims to design a decentralized, privacy-preserving intrusion detection system for Internet of Vehicles (IoV) environments while maintaining high accuracy and robust model performance.

🎯 Objectives:

1. Develop a CNN-based intrusion detection model for IoV network data.
2. Integrate the model within a federated learning framework to preserve data privacy across clients.
3. Evaluate model performance using accuracy, precision, recall, F1-score, and AUC metrics.
4. Compare results for both binary and multi-class classification scenarios.

⚙️ Federated Learning Configuration

The federated setup follows TensorFlow Federated (TFF) architecture with the following steps:

1. Model Initialization – The global CNN model is defined and broadcast to all clients.
2. Local Training – Each client trains its local CNN model using private data.
3. Model Aggregation – Local weights are securely aggregated on the central server.
4. Global Update – The updated global model is redistributed to clients.
5. Iteration – Steps 2–4 repeat for multiple rounds until convergence.

🧪 Dataset: CICIoV2024

The CICIoV2024 dataset is a recent and comprehensive dataset for intrusion detection in intra-vehicle networks.
It contains labeled CAN-bus traffic data representing normal and attack patterns across multiple vehicle ECUs.

Key Features:
1. Real-world IoV attack scenarios
2. Balanced and preprocessed features
3. Suitable for Federated Learning and CNN-based models

📊 Evaluation Metrics

The model performance is evaluated using:
1. Accuracy
2. Precision
3. Recall
4. F1-Score
5. Confusion Matrix
6. AUC Curve (Area Under ROC Curve)

Both binary and multi-class classification settings are supported.
