# CNN Projects

This repository contains implementations of convolutional neural network (CNN) architectures for the CIFAR-10 dataset using PyTorch and TensorFlow.

## AlexNet
- Implementation of the AlexNet architecture for the CIFAR-10 dataset in PyTorch and TensorFlow.

## VGG
- Implementation of the VGG architecture for the CIFAR-10 dataset in TensorFlow.

## Distributed Training with Data Parallelism
- Implementation of distributed training using data parallelism technique in PyTorch for the AlexNet architecture.

### Performance Comparison

| Batch Size | 1 GPU Time              | 1 GPU Test Accuracy | 2 GPUs Time             | 2 GPUs Test Accuracy |
|------------|-------------------------|---------------------|--------------------------|----------------------|
| 128        | 3 min 10 sec            | 72.8%               | 5 min 11 sec             | 73%                  |
| 256        | 3 min 05 sec            | 70%                 | 3 min 20 sec             | 70%                  |
| 512        | 3 min                   | 66.3%               | 2 min 27 sec             | 67.8%                |
| 1024       | 2 min 48 sec            | 60%                 | 1 min 57 sec             | 61%                  |
| 2048       | Out of Memory           | -                   | Out of Memory            | -                    |

Note: Out of memory error occurred for batch size 2048.

Additional Experiment:
- Training for 50 epochs with batch size 1024:
  - 1 GPU: 14 min 29 sec, 73% test accuracy
  - 2 GPUs: 9 min 53 sec, 73% test accuracy

The training with 2 GPUs was approximately 1.45 times faster than with 1 GPU.

This experiment confirms that increasing the batch size requires increasing the number of epochs to achieve good accuracy.
