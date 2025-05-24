Analysing CT-Scan Image
DATA from Kaggle

Medical Imaging Classifier with PyTorch

This project explores binary classification of CT scans with and without contrast using Convolutional Neural Network (CNN) deep learning model trained on the SIIM medical image dataset.

Data
The dataset consist of DICOM and TIFF-format CT image.
Labels indicate whether contrast was used (Contrast = True or False).
Images and metadata were loaded from /kaggle/input/siim-medical-images.
Train-test split: 90% training, 10% testing.
Images were preprocessed into shape (1, 256, 256) for CNN input.


ML Libraries and Models
NumPy, Pandas, Matplotlib
scikit-image for image loading
PyTorch for model training
sklearn for evaluation metrics


Model PyTorch CNN:
Two convolutional layers + max pooling
Two fully connected layers (last with 2 output nodes for binary classification)
ReLU activations and Adam optimizer

Training Results
Trained for 10 epochs
Final training loss: ~0.004
Test Accuracy: 50%

              precision    recall  f1-score   support
           0       0.50      0.60      0.55         5
           1       0.50      0.40      0.44         5
       accuracy                         0.50        10
