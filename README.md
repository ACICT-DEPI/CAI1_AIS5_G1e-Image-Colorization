# Image Colorization Project

This repository contains a project for image colorization using the U-Net architecture. The goal of this project is to predict RGB color channels from grayscale images.

## Overview

In this project, we used a U-Net model to transform grayscale images into color images. The model was trained on paired datasets of grayscale and color images. The input images were of size 224x224 with a single channel (grayscale), and the output images were of size 224x224 with three channels (RGB).

## Dataset

The dataset consists of two folders:
- **Gray Images**: Contains the grayscale input images (224x224, 1 channel).
- **Color Images**: Contains the corresponding color images (224x224, 3 channels).

## Model Architecture

The U-Net architecture is designed for image segmentation tasks but has been adapted here for colorization purposes. It consists of the following components:
- **Contracting Path**: Downsampling the input image while capturing context.
- **Bottleneck**: The deepest layer of the network, which holds the learned features.
- **Expansive Path**: Upsampling to reconstruct the image while preserving spatial information.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/image-colorization.git
   cd image-colorization
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the colorization model, use the following command:
```bash
python colorization.py --input_path path/to/gray/images --output_path path/to/save/color/images
```

Replace `path/to/gray/images` with the path to your grayscale images and `path/to/save/color/images` with the desired output path for the color images.

## Results

After training the model, you can evaluate its performance by checking the generated color images in the output folder.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgements

- U-Net Architecture: [Ronneberger et al. (2015)](https://arxiv.org/abs/1505.04597)
- Image Colorization Techniques