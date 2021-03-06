# Pneumonia X-rays Image Recognition
This is a project to practice use of CNNs for image recognition on pneumonia x-ray images

The dataset for this project contains chest x-ray images.
The dataset contains a training folder (5216 images), validation folder (16 images) and test folder (624 images).
The split of training and validation data here is a bit lopsided so training and validation sets will be adjusted.
These images are greyscale so will be represented by a [pixel_height, pixel width] matrix.
Some images, although being greyscale images, are in a RGB format so will have to be converted.
The images are for patients with bacterial pneumonia, viral pneumonia and no pneumonia.
To increase the amount of data, I experimented with using data augmentation.
This project will use a convolutional neural network to categorise these images.
The CNN will be based on LeNet, with some adjustments.

The layers of the model are as follows:
* a rescaling layer - this is used to normalize the inputs to the model
* a convolution layer - image detection
* a pooling layer - reducing the size of the representation to increase computation speed
* a convolution layer
* a pooling layer 
* a flatten layer - resizes data to 1d
* a relu layer - activation function
* a relu layer
* a softmax layer - for categorization

 It differs from LeNet by using same convolutions to maintain the size of images and max pooling layers instead of average pooling, which is more popular in modern deep learning
 
 I also did some experimention with dropout layers
