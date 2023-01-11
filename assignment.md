

IT3312 – AI TECHNOLOGIES

Assignment

In this individual assignment, you will perform image processing and implement Machine

Learning (ML) and Deep Learning (DL) models to solve a classification problem in Computer

Vision (CV). You will then tune each model accordingly to improve the performance of your

models. Having acquired the fundamental understanding of these models, you will then explore

powerful AI services provided by Google Cloud Vision API and propose an application to solve

any problem relating to CV. This assignment carries a total of 50 marks and constitutes 35% of

the module grade.

Schedule

. In week 16, your tutor will conduct a progress check

. In week 17, you will demo Part 1, 2 and 3 to your tutor

. Upload a zip file of your 4 Jupyter notebooks and 1 Word document to Brightspace by

end of week 17, Sun 14 Aug 2022, 2359h

Assignment Brief

Part 1 – Input Dataset

The original [CIFAR-10](https://www.cs.toronto.edu/%7Ekriz/cifar.html)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar.html)[dataset](https://www.cs.toronto.edu/%7Ekriz/cifar.html)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar.html)consists of 60,000 32x32 color images in 10 classes, with 6,000

images per class. There are 50,000 training images and 10,000 test images.

You will use black and white images converted from CIFAR-10 as your input dataset. Document

your work and results in a Jupyter notebook:

(1) Download the black and white source files [here](https://drive.google.com/drive/folders/1Df7euj71zGxIlpCM8DXmYvhu3dptkw9L?usp=sharing)

(2) Perform Exploratory Data Analysis (EDA) and discuss the input data

(3) Perform data normalization

(4) Derive the black and white images from the original color images

. Downloa[d](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[CIFAR-10](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[python](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[version](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[ ](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)[(color)](https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz)

. Understand the data structure

. Convert the first 50 color training images to black and white using the Python

Imaging Library

. Verify the black and white values are identical to (1)

Part 2 – Machine Learning

Build the following Machine Learning models to classify the input datasets, calculate the

performance metrics and document your work and results in a Jupyter notebook:

2022/S1 (Assignment)

Page 1 of 6





IT3312 – AI TECHNOLOGIES

(1) Logistic Regression

(2) Random Forest

For the better model, use the [Grid](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)[ ](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)[Search](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)[ ](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)[CV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)[ ](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)to determine the optimum set of

hyperparameters.

Part 3 – Deep Learning

Build a Convolution Neural Network (CNN) to classify the input dataset, calculate the

performance metrics and document your work and results in a Jupyter notebook:

(1) Build the following CNN model:

i.

Convolutional layer

Feature Maps: 32; Receptive field: 3 by 3; Activation: Relu

Max pooling layer

ii.

Pool size: 2 by 2

iii.

iv.

v.

Convolutional layer

Feature Maps: 64; Receptive field: 3 by 3; Activation: Relu

Max pooling layer

Pool size: 2 by 2

Convolutional layer

Feature Maps: 64; Receptive field: 3 by 3; Activation: Relu

Max pooling layer

vi.

Pool size: 2 by 2

vii.

Flatten layer

viii.

Fully connected (Dense) layer

Units: 64; Activation: Relu

Fully connected (Dense) output layer

Activation: Softmax

ix.

(2) Implement relevant techniques (covered in the lecture) to optimize your model.

Possible options include:

. Exploring data augmentation

. Tuning the hyperparameters (e.g. the number of layers) in your CNN

. Tuning the hyperparameters in Neural Networks

(3) Conclude the performance of the final model

(4) Analyse the effect of input data on performance

. Create a new model based on your final model in (3) and tweak it to accept inputs of

color images (3 channels)

. Train it using the original CIFAR-10 color training images

. Calculate the performance using CIFAR-10 color test images

. Explain why this model is better/worse than (3)

2022/S1 (Assignment)

Page 2 of 6





IT3312 – AI TECHNOLOGIES

Part 4 – AI Services

Google Cloud Vision API provides a set of services for analyzing images. Here are some

examples:

. Label Detection

. Text Detection

. Document Text Detection

. Facial Detection

. Landmark Detection

. Logo Detection

. Image Properties

Propose an application that uses one, two or three services to solve a problem relating to CV:

. You do not need to build a working prototype

. For each service you use, show your workings of the API (e.g. issuing request and

processing response) in a Jupyter notebook

. Describe any background research, challenges and assumptions in a Microsoft Word

document

2022/S1 (Assignment)

Page 3 of 6






IT3312 – AI TECHNOLOGIES

Rubrics

Criteria

F

C-D

(5-6)

B

(7-8)

A

(0-4)

(9-10)

Input Dataset

[8 Marks]

Exploratory Data

Analysis

• Poor understanding of

input data, data cleaning

and relationship between

variables

• Moderate understanding • Good understanding of

• Excellent understanding

of input data, data

cleaning and relationship

between variables

• Excellent statistical

analysis

of input data, data

cleaning and relationship

between variables

• Moderate statistical

analysis

input data, data cleaning

and relationship between

variables

• Poor statistical analysis

• Good statistical analysis

Input Processing

• No/Poor derivation

• Poor understanding of

conversion process

• Partial derivation

• Moderate understanding • Good understanding of

of conversion process

• Good derivation

• Full derivation

• Excellent understanding

of conversion process

conversion process

Machine Learning

[8 Marks]

Models Creation

and Analysis

• Models do not work

• Poor understanding of

performance metrics

• Models partially work

• Moderate understanding • Good understanding of

of performance metrics

• Models mostly work

• Models fully work

• Excellent understanding

of performance metrics

performance metrics

Hyperparameters

Tuning using Grid

Search

• Poor knowledge of Grid

Search

• Poor understanding of

tuning hyperparameters

• Moderate knowledge of

Grid Search

• Moderate understanding • Good understanding of

of tuning

• Good knowledge of Grid

Search

• Excellent knowledge of

Grid Search

• Excellent understanding

of tuning

tuning hyperparameters

hyperparameters

hyperparameters

2022/S1 (Assignment)

Page 4 of 6





IT3312 – AI TECHNOLOGIES

Deep Learning

[15 Marks]

Models Creation

and Performance

• Model is not constructed • Model is partially

• Model is mostly

constructed according to

specifications

• Model is fully constructed

according to

specifications

according to

specifications

constructed according to

specifications

Hyperparameters

Tuning

• Poor knowledge in tuning • Moderate knowledge in

• Good knowledge in

tuning hyperparameters

and implementation of

optimization techniques

• Excellent knowledge in

tuning hyperparameters

and implementation of

optimization techniques

hyperparameters and

implementation of

tuning hyperparameters

and implementation of

optimization techniques

optimization techniques

Processing Color

Images

• Model does not work

• Poor understanding of DL • Moderate understanding • Good understanding of

concepts

• Model partially works

• Model mostly works

• Model fully works

• Excellent understanding

of DL concepts

of DL concepts

DL concepts

AI Services

[10 Marks]

Innovation and

Feasibility

• Application has no real

benefits or positive

impact

• Application has minimal

benefits or positive

impact

• Application has moderate • Application has huge

benefits or positive

impact

benefits or positive

impact

• Application has no

feasible elements

• Application has a few

feasible elements

• Application has some

feasible elements

• Application has many

feasible elements

Application of APIs • Little understanding on

• Partial understanding on

the APIs used

• Good understanding on

the APIs used

• Thorough understanding

on the APIs used

the APIs used

• Unable to interface to the • Able to interface to some • Able to interface to most • Able to interface to all the

APIs

of the APIs

of the APIs

APIs

Report Structure

and Content

• Content is poorly

organized and lacking a

logical flow of ideas

• Content is partially

organized with a logical

flow of ideas and some

ideas are conveyed

• Content is mostly

organized with a logical

flow of ideas and most

ideas are conveyed

• Content is well organized

with a clear and logical

flow of ideas and all ideas

are clearly conveyed

2022/S1 (Assignment)

Page 5 of 6





IT3312 – AI TECHNOLOGIES

• Poor use of language with • Partial use of language

• Good use of language

with no grammar and

spelling mistakes

• Excellent use of language

with no grammar and

spelling mistakes

many grammar and

spelling mistakes

with some grammar and

spelling mistakes

Source Codes &

Demo

[9 Marks]

Notebooks

Structure and

Content

• Content is poorly

organized

• Poor use of Markdown to • Moderate use of

explain processes

• Poor use of comments in

codes

• Content is moderately

organized

• Content is mostly

organized

• Good use of Markdown

to explain processes

• Good use of comments in • Excellent use of

codes

• Content is well organized

• Excellent use of

Markdown to explain

processes

Markdown to explain

processes

• Moderate use of

comments in codes

comments in codes

Demo

• Content meets less than

50% of the objectives

• Poor subject knowledge

and understanding of

codes

• Content meets 50% to

74% of the objectives

• Moderate subject

knowledge and

• Content meets 75% to

89% of the objectives

• Good subject knowledge

and understanding of

codes

• Content meets 90% or

more of the objectives

• Excellent subject

knowledge and

understanding of codes

understanding of codes

2022/S1 (Assignment)

Page 6 of 6

