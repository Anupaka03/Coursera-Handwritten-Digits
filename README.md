# GAN for Handwritten Digit Generation
 Deep Learning with PyTorch - Handwritten digits using GAN guided project offered by Coursera.
 This project implements a Generative Adversarial Network (GAN) to generate handwritten digits resembling those from the MNIST dataset. The model uses a Discriminator and Generator network, trained with the BCEWithLogits loss function and the Adam optimizer.

 ## Introduction
This project demonstrates the use of a GAN to generate synthetic images of handwritten digits. The GAN comprises two neural networks: the Generator, which creates images, and the Discriminator, which evaluates them. The training process involves both networks competing to improve their respective performances.

## Dataset
The MNIST dataset is used for training, containing 60,000 training images and 10,000 test images of handwritten digits (0-9), each sized 28x28 pixels.

## Model Architecture
### Generator
The Generator network takes a noise vector as input and generates a 28x28 pixel image. It uses transposed convolutional layers for upsampling the noise vector to the desired image size.
### Discriminator
The Discriminator network takes a 28x28 pixel image as input and outputs a probability indicating whether the image is real or fake. It uses convolutional layers followed by batch normalization and leaky ReLU activations.

## Training
The model is trained using the BCEWithLogits loss function for both the Discriminator and Generator networks, with the Adam optimizer for optimization.

## Results
After training, the model achieves a Discriminator loss of approximately 0.52 and a Generator loss of approximately 0.003. The generated images resemble handwritten digits from the MNIST dataset.
