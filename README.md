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
4. Derive the black and white images from the original color images
    1. Download [CIFAR-10 python version (color)](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)
    2. Understand the data structure
    3. Convert the first 50 color training images to black and white using the Python Imaging Library
    4. Verify the black and white values are identical to (1)


Part 2 – Machine Learning

Build the following Machine Learning models to classify the input datasets, calculate the performance metrics and document your work and results in a Jupyter notebook:
1. Logistic Regression
2. Random Forest

For the better model, use the [CIFAR-10 dataset](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) to determine the optimum set of hyperparameters.


Part 3 – Deep Learning

Build a Convolution Neural Network (CNN) to classify the input dataset, calculate the performance metrics and document your work and results in a Jupyter notebook:
1. Build the following CNN model:
    1. Convolutional layer
        1. Feature Maps: 32; Receptive field: 3 by 3; Activation: Relu
    2. Max pooling layer
        1. Pool size: 2 by 2
    3. Convolutional layer
        1. Feature Maps: 64; Receptive field: 3 by 3; Activation: Relu
    4. Max pooling layer
        1. Pool size: 2 by 2
    5. Convolutional layer
        1. Feature Maps: 64; Receptive field: 3 by 3; Activation: Relu
    6. Max pooling layer
        1. Pool size: 2 by 2
    7. Flatten layer
    8. Fully connected (Dense) layer
        1. Units: 64; Activation: Relu
    9. Fully connected (Dense) output layer
        1. Activation: Softmax 
2. Implement relevant techniques (covered in the lecture) to optimize your model. 
Possible options include:
    1. Exploring data augmentation
    2. Tuning the hyperparameters (e.g. the number of layers) in your CNN
    3. Tuning the hyperparameters in Neural Networks
3. Conclude the performance of the final model
4. Analyse the effect of input data on performance
    1. Create a new model based on your final model in (3) and tweak it to accept inputs of color images (3 channels)
    2. Train it using the original CIFAR-10 color training images
    3. Calculate the performance using CIFAR-10 color test images
    4. Explain why this model is better/worse than (3)


Part 4 – AI Services

Google Cloud Vision API provides a set of services for analyzing images. Here are some examples:
