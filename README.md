# Hopfield Network from Scratch

This is a Python notebook where I implemented the training and prediction process of a Hopfield Network using a dataset of images. The Hopfield network is a form of recurrent artificial neural network that can serve as associative memory, storing and recalling patterns.

## Overview

In this project, I trained a Hopfield Network on binary images derived from a dataset, stored patterns in the weight matrix, and performed pattern recovery in the presence of noise. The main steps include:

* Converting RGB images to binary.
* Storing image patterns in a weight matrix.
* Adding noise to images.
* Reconstructing the original image using the Hopfield dynamics.

## Requirements

- Python 3.x
- Numpy 
- Matplotlib
- PIL

You can install the required packages with the following command:
```bash
pip install numpy matplotlib pillow
```

## Explanation

Our dataset consists of vectors **x**, each of dimension **1 × (m × n)**, where **m** and **n** are the height and width of the images, respectively. The weight matrix is computed as the outer product of these vectors.

The weight matrix is defined as:

$$
\mathbf{W} = \sum_{i=1}^{N} \mathbf{x}_i \mathbf{x}_i^T \ .
$$

The update rule for the system is: 

$$
\boldsymbol{\xi}^{t+1} = \text{sgn}(\boldsymbol{W} \boldsymbol{\xi}^t - \boldsymbol{b}) \ 
$$



## Resources

[Hopfield network theory](https://ml-jku.github.io/hopfield-layers/#beyond)

[CelebA dataset](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset)


