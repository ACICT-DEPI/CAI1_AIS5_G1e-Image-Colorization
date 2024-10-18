# Image Colorization Project

This repository contains a project for image colorization using the U-Net architecture. The goal of this project is to predict RGB color channels from grayscale images.

## Overview

In this project, we used a U-Net model to predict RGB channels. The model was trained on paired datasets of grayscale and color images. The input images were of size 224x224 with a single channel (grayscale), and the output images were of size 224x224 with three channels (RGB).

## Dataset

The dataset consists of two folders:
- **Gray Images**: Contains the grayscale input images (224x224, 1 channel).
- **Color Images**: Contains the corresponding color images (224x224, 3 channels).

## Model Architecture

The U-Net architecture is designed for image segmentation tasks but has been adapted here for colorization purposes. It consists of the following components:
- **Contracting Path**: Downsampling the input image while capturing context.
- **Bottleneck**: The deepest layer of the network, which holds the learned features.
- **Expansive Path**: Upsampling to reconstruct the image while preserving spatial information.
## Data
- [Kaggle DataSet](https://www.kaggle.com/datasets/theblackmamba31/landscape-image-colorization)
- [Kaggle Notebook](https://www.kaggle.com/code/aliabdelmenam/image-colorization-u-net)
## Deployment
- Deploy model using streamlit 

## Model
-  [Model](https://www.kaggle.com/models/aliabdelmenam/keras_model/)
-  Model as in `Pickle` file  
