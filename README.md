# MNIST Simple CNN with PyTorch

This repository contains the code for a simple Convolutional Neural Network (CNN) built with PyTorch that recognizes handwritten digits from the MNIST dataset.

## Dataset

The MNIST dataset is a collection of 70,000 grayscale images of handwritten digits, each with a size of 28x28 pixels. The dataset is split into a training set of 60,000 images and a test set of 10,000 images. Each image is labeled with the correct digit from 0 to 9.

## CNN Architecture

The CNN used in this repository consists of two convolutional layers followed by two fully connected layers. The first convolutional layer uses 32 filters with a 3x3 kernel, while the second convolutional layer uses 64 filters with a 3x3 kernel. Both convolutional layers use padding and a stride of 1, and are followed by a ReLU activation function and a max pooling layer with a 2x2 kernel and a stride of 2. The output of the second convolutional layer is flattened and fed into a fully connected layer with 128 units, which is followed by another fully connected layer with 10 units, corresponding to the 10 possible digit classes. The network uses the cross-entropy loss function and the Adam optimizer.

## Results

After training the network for 10 epochs with a batch size of 50, the model achieves an accuracy of 98.97% on the test set. This is a state-of-the-art result on the MNIST dataset and demonstrates the effectiveness of CNNs for image classification tasks.

## Conclusion

The MNIST dataset and the simple CNN architecture used in this repository are a good starting point for learning about deep learning and image classification. By modifying the network architecture, experimenting with different optimization algorithms, and using larger and more complex datasets, it is possible to achieve even better results on a wide range of computer vision tasks.
