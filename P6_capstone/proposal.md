# Machine Learning Engineer Nanodegree
## Capstone Proposal
Jiaxi Yuan  
August 7th, 2018

### Domain Background

Due to the high speed development of machine learning, this techinique has been used across our daily life. For example, autonoumous driving, which is an unimaginable concept maybe 15 years ago, is applied to real life and mature products have been manufactured to the market. However, machine learning is not only something far away or expensive to get in touch, we can find it everywhere now, such as the intelligent recommnedation of the music app and also what will be mainly discussed here -- traffic sign recognition.

Traffic sign is what we can see everyday, especailly for those who need to drive. Traffic sign includes different types, such as stop sign, speed limit sign. Due to my personal interest in autonomous driving, I did a lot of research on what kind of techniques needed. The traffic sign recognition is one of the most basic and necessary part for the self-driving car. It needs the support of machine learning with enough data set.

### Problem Statement

The prblem to be investigated here is how to use machine learning to realized traffic sign recognition. German traffic sign dataset will be used as both training data and testing data. Some image processing needs to be done so that all the images can be better used as the input. Image augmentation might need to be done for the better recognition performance. For the model architecture, deep learning will be first considered.

### Datasets and Inputs

The dataset is called GTSRB, known as German Traffic Sign Recognition Benchmark. GTSRB is a multi-class, single-image classification challenge held at the International Joint Conference on Neural Networks (IJCNN) 2011. 

The images contain one traffic sign each. They contain a border of 10 % around the actual traffic sign (at least 5 pixels) to allow for edge-based approaches. The image size vart between 15*15 to 250*250 pixels. Each image has an annotation which includes:
-Filename: Filename of corresponding image
-Width: Width of the image
-Height: Height of the image
-ROI.x1: X-coordinate of top-left corner of traffic sign bounding box
-ROI.y1: Y-coordinate of top-left corner of traffic sign bounding box
-ROI.x2: X-coordinate of bottom-right corner of traffic sign bounding box
-ROI.y2: Y-coordinate of bottom-right corner of traffic sign bounding box
-ClassID: Assigned class label

### Solution Statement

First, the data set will be loaded and be split into training and testing data. As each input data has a label, supervised learning will be applied. In order to have the best results, different training methods will be tried, such as K-nearest, SVM, deep learning. After training, the model will be applied to the testing data and get the accuracy.

### Benchmark Model

A Kaggle competition called Digit Recongnizer can be used as the benchmark. The dataset provided is much less than the dataset provided by MNIST. The good accuracy can reach to over 99%. The result can be used as the benchmark of this project.

### Evaluation Metrics

As mentioned above, the top Kaggle competitioners can make the accuracy to over 99%. I'll use this as a target. At least 95% of the accuracy rate is expected. And the best training method with the best performance will be reported finally. 

### Project Design

1. Data preprocessing: Load the the MNIST data, perform some preprocessing to the data. Split the data into training data and testing data.
2. Training: Different training methods will be tried, such as K-nearest, SVM, CNN, deep learning with diffrent layer combinations.  After the training, the model will be applied to testing data..
3. Testing and optimizing: Apply the trained model to the testing data and get the final accuracy of different models. Find the best way to do digit recognition. After choosing the best model, try different parameters to optimize the model.
