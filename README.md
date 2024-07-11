# PatchPal - A satellite image segmentation model 
PatchPal is a semantic segmentation model designed to classify and segment satellite images into various land cover classes such as water, land, road, building, and vegetation. This project leverages the U-Net architecture to achieve accurate segmentation, facilitating applications in urban planning, environmental monitoring, and disaster management.

## Overview
Semantic segmentation involves labeling each pixel of an image with a class, enabling detailed understanding of the scene. PatchPal is trained on satellite images to identify and segment different land cover types.

## Features 
- Semantic Segmentation: Classifies and segments satellite images into multiple land cover classes.
- U-Net Architecture: Utilizes a U-Net model for efficient and accurate segmentation.
- Custom Evaluation Metric: Includes Jaccard Coefficient (IoU) for evaluating segmentation performance.
- Class Imbalance Handling: Implements focal loss to address class imbalance in the dataset.

## Tech Stack 
TensorFlow: For model building and training.
Keras: For high-level neural network API.
NumPy: For data manipulation.
Matplotlib: For visualization.

## Model Archtecture 
The U-Net model used in PatchPal consists of an encoder-decoder structure with the following layers:

Encoder: Series of Conv2D, Dropout, and MaxPooling2D layers to extract features.
Bottleneck: Deepest part of the network, capturing the most abstract features.
Decoder: Series of Conv2DTranspose, concatenate, and Conv2D layers to reconstruct the image and produce segmentation masks
