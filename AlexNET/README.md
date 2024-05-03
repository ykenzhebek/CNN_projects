# AlexNet Overview

## Introduction
AlexNet is a deep convolutional neural network (CNN) that was presented by Alex Krizhevsky, Ilya Sutskever, and Geoffrey Hinton in 2012. This architecture played a pivotal role in advancing the deep learning field by winning the ImageNet Large Scale Visual Recognition Challenge (ILSVRC) in 2012.

![AlexNet Architecture](https://github.com/KenzhebekYerzhan/aiBoost/blob/main/AlexNET/alexnet-tensorflow/architecture.png)
## Key Features
- **Depth**: Contains eight layers; five convolutional and three fully connected layers.
- **ReLU Activation**: Introduced the use of the Rectified Linear Activation function, which helped in faster training.
- **Dropout**: Used dropout layers to prevent overfitting, which was a novel concept at the time.
- **Overlapping Max-Pooling**: Used overlapping pooling layers which reduced the size of the network.
- **Data Augmentation**: Employed data augmentation techniques to artificially increase the size of the training set.
- **GPU Training**: Designed to be trained on two GPUs, due to the limited memory of GPUs at that time.

## Achievements
AlexNet achieved a top-5 error rate of 15.3% on the ImageNet ILSVRC-2010 dataset, a significant improvement over previous models.

## Reference
Krizhevsky, A., Sutskever, I., & Hinton, G. E. (2012). ImageNet classification with deep convolutional neural networks. In Advances in neural information processing systems (pp. 1097-1105).
