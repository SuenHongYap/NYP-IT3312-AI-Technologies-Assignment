# NYP-IT3312-AI-Technologies-Assignment
In this individual assignment, you will perform image processing and implement Machine
Learning (ML) and Deep Learning (DL) models to solve a classification problem in Computer
Vision (CV). You will then tune each model accordingly to improve the performance of your
models. Having acquired the fundamental understanding of these models, you will then explore
powerful AI services provided by Google Cloud Vision API and propose an application to solve
any problem relating to CV.

# Assignment Brief

Part 1 – Input Dataset

The original [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) consists of 60,000 32x32 color images in 10 classes, with 6,000
images per class. There are 50,000 training images and 10,000 test images.

You will use `black and white` images converted from CIFAR-10 as your input dataset. Document
your work and results in a Jupyter notebook:
1. Download the black and white source files [here](https://drive.google.com/drive/folders/1Df7euj71zGxIlpCM8DXmYvhu3dptkw9L).
2. Perform Exploratory Data Analysis (EDA) and discuss the input data
3. Perform data normalization

(4) Derive the black and white images from the original color images
  1. Download CIFAR-10 python version (color)
  2. Understand the data structure
  3. Convert the first 50 color training images to black and white using the Python Imaging Library
  4. Verify the black and white values are identical to (1)
