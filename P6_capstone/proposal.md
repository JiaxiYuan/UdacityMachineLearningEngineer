# Machine Learning Engineer Nanodegree
## Capstone Proposal
Jiaxi Yuan  
August 7th, 2018

### Domain Background

Due to the high speed development of machine learning, this techinique has been used across our daily life. For example, autonoumous driving, which is an unimaginable concept maybe 15 years ago, is applied to real life and mature products have been manufactured to the market. However, machine learning is not only something far away or expensive to get in touch, we can find it everywhere now, such as the intelligent recommnedation of the music app and also what will be mainly discussed here -- Digit Reconginition.

Digits used worldwide are only comprised of 10 different characters, 0~9. It seems pretty simple to reconginize, espeacially when its the printed digit. However, when it comes to handwrite digits, the reconginition process will become more complicated. Differnt people have different writing styles. Or even, people from different areas or countries have different ways writing digits. With the help of machine learning, this problem can be resolved for computer to reconginize human writing digits.

### Problem Statement

The prblem to be investigated here is how to use machine learning to realized handwritten digits recognition. MINIST dataset will be used as both training data and testing data. Differnt training methods will be appied, such as SVM, CNN, deep learning. After applying the model to testing data, a accuracy comparison will be done between different models to see which one has the best result. Some preprocessing of the input data might be done before training.

### Datasets and Inputs

The dataset is called MNIST, provided by Yann LeCun, Corinna Cortes and Christopher Burges. The dataset is used for evaluating machine learning models on the handwritten digit classification problem. Images of digits were taken from a variety of scanned documents, normalized in size and centered.

Each image is a 28 by 28 pixel square. For each image, there's a label represeting the 10 digits or 10 classes.

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
