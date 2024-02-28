# Detection of Digital Face Manipulation

This project aims to detect manipulated/fake face images and videos using deep learning techniques. 

## Overview

With advancing image and video generation methods, it has become easier to create manipulated media that can potentially spread false information. This project classifies an input face image/video as real or fake using convolutional and recurrent neural networks.

Key functionality:

- Scan input image and face detection
- Train models on dataset of real and fake images 
- Compare input face to trained dataset
- Classify face as real or manipulated

## Getting Started

### Prerequisites

Requirements to run this project:

- Python 3
- OpenCV 
- NumPy
- TensorFlow/Keras

### Usage

The entry point script for running predictions is `predict.py`. Sample usage:

```
python predict.py --input_file sample_input.jpg
```

This will run the trained model on the given input file and print the prediction of real vs fake.

The training script is `train.py` which trains a model on the dataset and saves the model for later use.

## Dataset

The dataset used for training models is available in the `dataset` directory. It contains real and fake images scraped from open sources.
