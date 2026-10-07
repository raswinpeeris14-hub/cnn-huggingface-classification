# cnn-huggingface-classification
Image classification using CNN and a Hugging Face CIFAR-10 dataset.
Project Overview
This project implements Image Classification using a Convolutional Neural Network (CNN) with a CIFAR-10 image dataset obtained from the Hugging Face Hub.

The CNN model is trained to classify images into 10 different categories.

🎯 Objectives
Load an image dataset from Hugging Face.

Preprocess and normalize the images.

Build a Convolutional Neural Network using TensorFlow/Keras.

Train the CNN model on the dataset.

Evaluate the model using test data.

Display accuracy and loss graphs.

Generate predictions for test images.

Generate a classification report and confusion matrix.

📊 Dataset
The project uses the CIFAR-10 dataset.

The dataset contains 60,000 color images belonging to 10 classes:

Class	Description
0	Airplane
1	Automobile
2	Bird
3	Cat
4	Deer
5	Dog
6	Frog
7	Horse
8	Ship
9	Truck

Dataset source:

Hugging Face:
https://huggingface.co/datasets/rajnandinib/CIFAR10

The images are RGB images with a size of 32 × 32 pixels.

🧠 CNN Architecture
The model consists of the following layers:

Input Image
    ↓
Conv2D (32 filters)
    ↓
MaxPooling2D
    ↓
Conv2D (64 filters)
    ↓
MaxPooling2D
    ↓
Conv2D (128 filters)
    ↓
MaxPooling2D
    ↓
Flatten
    ↓
Dense (128 neurons)
    ↓
Dropout
    ↓
Dense (10 neurons)
    ↓
Softmax
    ↓
Predicted Class

🛠️ Technologies Used
Python

TensorFlow

Keras

Hugging Face Datasets

NumPy

Matplotlib

Scikit-learn

📁 Project Structure
cnn-huggingface-classification/
│
├── cnn_classification.py
├── requirements.txt
├── README.md
└── .gitignore

⚙️ Installation
Clone this repository:

git clone https://github.com/YOUR_USERNAME/cnn-huggingface-image-classification.git

Move into the project directory:

cd cnn-huggingface-image-classification

Install the required libraries:

pip install -r requirements.txt

▶️ How to Run
Run the Python program:

python cnn_classification.py

The program will:

Download the dataset from Hugging Face.

Convert the images into NumPy arrays.

Normalize the image pixels.

Create the CNN model.

Train the model.

Evaluate the model.

Display accuracy and loss graphs.

Predict test images.

Generate a classification report.

Display the confusion matrix.

📈 Model Evaluation
The model is evaluated using:

Training accuracy

Validation accuracy

Test accuracy

Training loss

Validation loss

Classification report

Confusion matrix

Example:

Test Accuracy: 0.70

Note: The actual accuracy may vary depending on the training environment, TensorFlow version, random initialization, and training parameters.

🔍 Prediction
The model predicts the class of an image using the Softmax output layer.

Example:

Predicted: cat
Actual: cat

📊 Output
The program generates:

Accuracy Graph
Shows the training and validation accuracy over the training epochs.

Loss Graph
Shows the training and validation loss.

Classification Report
Provides:

Precision

Recall

F1-score

Support

Confusion Matrix
Shows the number of correctly and incorrectly classified images for each class.

🚀 Future Improvements
The project can be improved by:

Increasing the number of CNN layers.

Using data augmentation.

Using Batch Normalization.

Applying Transfer Learning.

Increasing the number of training epochs.

Using models such as ResNet or MobileNet.

Deploying the trained model as a web application.
