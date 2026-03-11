CNN Model Accuracy & Loss Testing on MNIST Dataset

Project Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify handwritten digits from the MNIST dataset.
The goal of this project is to train a deep learning model, evaluate its performance, and analyze classification results using metrics such as accuracy, loss, classification report, and confusion matrix.

The project also visualizes misclassified images to better understand the model’s prediction errors.

⸻

Dataset

The model uses the MNIST dataset, which is a standard benchmark dataset for image classification.

Dataset Details
	•	70,000 grayscale images of handwritten digits
	•	Image size: 28 × 28 pixels
	•	10 classes (digits 0–9)

Split used in the project:
	•	Training samples: 60,000
	•	Testing samples: 10,000

  
Model Compilation
The model is compiled with:
	•	Optimizer: Adam
	•	Learning Rate: 0.0005
	•	Loss Function: Sparse Categorical Crossentropy
	•	Metric: Accuracy


Training Configuration
	•	Epochs: 10
	•	Batch Size: 128
	•	Validation Split: 20%

Early stopping is used to prevent overfitting.

Model Evaluation

After training, the model is evaluated on the test dataset.

Results
	•	Test Accuracy: ~98.6%
	•	Test Loss: ~0.046


Performance Metrics

1. Classification Report

The classification report provides:
	•	Precision
	•	Recall
	•	F1-score
	•	Support

for each digit class (0–9).


2. Confusion Matrix

The confusion matrix shows how often digits are misclassified.

Example interpretation:
	•	Most predictions fall on the diagonal (correct predictions).
	•	Few misclassifications occur between visually similar digits such as 4 and 6 or 6 and 8.


Misclassified Image Visualization

The project also displays misclassified digits to analyze model errors.


