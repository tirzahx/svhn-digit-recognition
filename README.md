# Handwritten Digit Recognition (SVHN Dataset)

This project implements a Convolutional Neural Network (CNN) to classify digits (0–9) from the **Street View House Numbers (SVHN)** dataset.  
Unlike MNIST, SVHN is a more realistic and challenging dataset, containing digits from natural scene images (house numbers).

## Features
- Preprocessed SVHN dataset (normalization, batching, shuffling).
- CNN model with multiple convolutional + pooling layers.
- Regularization with dropout to prevent overfitting.
- Achieved **~91% test accuracy**.
- Implemented in Python with TensorFlow/Keras.

## Model Architecture
- Conv2D (32 filters, 3×3, ReLU) + MaxPooling  
- Conv2D (64 filters, 3×3, ReLU) + MaxPooling  
- Conv2D (128 filters, 3×3, ReLU)  
- Flatten → Dense (128, ReLU)  
- Dropout (0.5)  
- Dense (10, Softmax)  

## Training Details
- Optimizer: Adam (lr=0.001)  
- Loss: Sparse Categorical Crossentropy  
- Batch size: 64  
- Epochs: 15  
- Framework: TensorFlow/Keras  


## Results
- Training Accuracy: ~90%  
- Test Accuracy: ~91%  
- Model generalized well despite noisy and cluttered images.


## How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/svhn-digit-recognition.git
   cd svhn-digit-recognition
