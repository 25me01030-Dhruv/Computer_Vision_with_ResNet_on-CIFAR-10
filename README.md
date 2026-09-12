Computer Vision with ResNet-18 on CIFAR-10
Overview

This project implements a ResNet-18 convolutional neural network from scratch for image classification on the CIFAR-10 dataset. The model was developed using PyTorch and trained on a NVIDIA T4 GPU through Google Colab.

The objective was to understand and implement the architecture of a residual neural network while evaluating its performance on a standard computer vision benchmark.

Model & Training Configuration

The ResNet-18 architecture was implemented from scratch using PyTorch. The training pipeline was configured with the following hyperparameters:

Dataset: CIFAR-10
Architecture: ResNet-18
Framework: PyTorch
Hardware: NVIDIA T4 GPU
Optimizer: Stochastic Gradient Descent (SGD)
Learning Rate: 0.1
Batch Size: 200
Loss Function: Cross-Entropy Loss
Number of Epochs: 10
Results

Under the above training configuration, the model achieved:

Training Accuracy: 81.43%
Test Accuracy: 77.83%

Training performance was monitored throughout the process using visualizations of:

Epochs vs. Training/Test Accuracy
Epochs vs. Training/Test Loss

These plots provide an overview of the model's learning progression and generalization performance.

Understanding ResNet

Residual Network (ResNet) is a deep convolutional neural network architecture introduced in the 2015 paper Deep Residual Learning for Image Recognition. The architecture was designed to address the optimization difficulties encountered when training very deep neural networks.

The Vanishing Gradient Problem

As neural networks become deeper, gradients propagated backward during training can become extremely small. This can prevent earlier layers from receiving meaningful updates, making optimization increasingly difficult.

Importantly, this phenomenon is related to optimization degradation and vanishing gradients, rather than simply being a consequence of overfitting.

The ResNet Solution: Skip Connections

ResNet introduced residual/skip connections, which allow information to bypass one or more layers and flow directly toward deeper layers.

Instead of directly learning a desired mapping:

H(x) = F(x)

a residual block learns:

H(x) = F(x) + x

where:

x is the input to the residual block
F(x) represents the transformation learned by the convolutional layers
F(x) + x represents the resulting residual mapping

The skip connection provides an alternative pathway for both information and gradients, making the optimization of deeper networks more effective.

Significance

ResNet demonstrated that substantially deeper neural networks could be trained successfully without the degradation problems associated with increasing network depth. ResNet architectures subsequently became highly influential in computer vision and achieved strong performance on benchmarks such as ImageNet.

This project provided practical experience with:

Convolutional Neural Networks
Residual learning and skip connections
PyTorch model implementation
Image classification
Model training and evaluation
GPU-based deep learning
Performance visualization

