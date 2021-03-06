# Pneumonia X-rays Image Recognition
This is a project to practice use of CNNs for image recognition on pneumonia x-ray images

The dataset for this project contains chest x-ray images.
The dataset contains a training folder (5216 images), validation folder (16 images) and test folder (624 images).
The split of training and validation data here is a bit lopsided so training and validation sets will be adjusted.
These images are greyscale so will be represented by a [pixel_height, pixel width] matrix.
Some images, although being greyscale images, are in a RGB format so will have to be converted.
The images are for patients with bacterial pneumonia, viral pneumonia and no pneumonia.
To increase the amount of data, data augmentation will be used.
This project will use a convolutional neural network to categorise these images.
The CNN will be based on LeNet, with some adjustments.
