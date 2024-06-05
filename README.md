# Convolutional Autoencoder for Dog Images

## Overview

This project implements a convolutional autoencoder using the FastAI library to perform tasks like image denoising, dimensionality reduction, and clustering on a dataset of dog images.

## What is a Convolutional Autoencoder?

A convolutional autoencoder is a type of neural network that combines convolutional layers with autoencoder principles to learn efficient representations of input data. It is commonly used for unsupervised learning tasks such as image denoising, inpainting, and dimensionality reduction.

## Project Steps

1. **Importing Libraries**
2. **Loading and Preprocessing Data**
    - Used FastAI `DataLoaders` to preprocess and load data.
3. **Creating the Autoencoder Model**
    - Defined the autoencoder architecture with separate encoder and decoder parts.
4. **Creating the Learner**
    - Used FastAI `Learner` object with the model, data loaders, MSE loss function, Adam optimizer, and callback for saving the best model.
5. **Training the Autoencoder**
    - Trained the model and saved the best version.
6. **Inference and Testing**
    - Tested the model on dog images and visualized results.
7. **Dimensionality Reduction**
    - Used UMAP and t-SNE to reduce embedding dimensions and visualized results.
8. **Clustering on Embeddings**
    - Applied `SpectralClustering` and `NearestNeighbors` from scikit-learn on the autoencoder's embeddings.

## Installation

```sh
pip install fastai==2.7.9
pip install torch==1.12.1
pip install graphviz
pip install torchview
pip install umap-learn
