# VLG-submission-
Project Overview

This project implements an image classification model using PyTorch and a pre-trained ResNet-18 architecture. The aim is to sort images from a dataset with classes already specified and deliver a .csv file. 

Code Structure and Implementation:

1. Libraries and Imports:
The project uses the following key libraries:
torch: For model definition, training, and optimization.
torchvision: For pre-trained models and data transformations.
PIL: For image processing.
os and pandas: For dataset handling.

2. Dataset Preparation
Data Location:
Training data: train_folder = "C:\\Users\\Lenovo\\Desktop\\vlg-dataset\\train"
Testing data: test_folder = "C:\\Users\\Lenovo\\Desktop\\vlg-dataset\\test"

3. Transformations:
Resizing, normalization, and augmentation applied using torchvision.transforms.
Loaded via torchvision.datasets.ImageFolder.

4. Model Architecture
ResNet-18:
A pre-trained ResNet-18 model was used from torchvision.models.
The final fully connected layer was modified to match the number of classes in the dataset.

5. Training 
Loss Function: Cross-Entropy Loss (nn.CrossEntropyLoss).
Optimizer: Adam Optimizer (optim.Adam) with a learning rate of 0.0001.
Training Parameters: 20 Epochs and 64 batch size 

7. Hardware Used: personal laptop (13th gen Intel i7 and Nvidia RTX 4060 laptop version)

6. Evaluation
Metrics: 0.56702 accuracy 

