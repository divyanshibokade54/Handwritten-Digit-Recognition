# Handwritten Digit Recognition using Deep Learning

A deep learning project for recognizing handwritten digits (0-9) using the MNIST dataset. This repository implements and compares two neural network architectures: **CNN** and **ResNet**.

## Project Overview

This project demonstrates the implementation of deep learning models for handwritten digit classification, achieving high accuracy on the MNIST dataset.

### Models Implemented

1. **CNN Model** (`HDR_CNN_Model(G14).ipynb`)
   - Convolutional Neural Network architecture
   - Conv2D → MaxPooling → Conv2D → MaxPooling → Dense layers
   - Uses ReLU activation with Softmax output
   - Trained for 5 epochs

2. **ResNet Model** (`HDR_ResNet__Model(G14).ipynb`)
   - Baseline LeNet-5 architecture
   - Improved ResNet with residual blocks
   - Includes Batch Normalization
   - Trained for 10 epochs

## Dataset

- **MNIST Dataset**: 70,000 grayscale images of handwritten digits (28x28 pixels)
  - Training set: 60,000 images
  - Test set: 10,000 images

## Requirements

```
tensorflow
numpy
matplotlib
opencv-python
pillow
```

## Installation

```bash
pip install tensorflow numpy matplotlib opencv-python pillow
```

## Usage

1. Open the notebook in Google Colab or Jupyter Notebook
2. Run all cells sequentially
3. The model will train on MNIST data
4. Test with your own handwritten digit images

## Project Structure

```
BMDL_HDR_TAE/
├── HDR_CNN_Model(G14).ipynb    # CNN implementation
├── HDR_ResNet__Model(G14).ipynb # ResNet implementation
├── train.csv                    # Training data
├── test.csv                     # Test data
└── README.md                    # This file
```

## Model Architecture

### CNN Model
```
Input (28x28x1) → Conv2D(32) → MaxPool → Conv2D(64) → MaxPool → Flatten → Dense(128) → Dense(10)
```

### ResNet Model
```
Input (28x28x1) → ResBlock(32) → MaxPool → ResBlock(64) → MaxPool → Flatten → Dense(128) → Dense(10)
```

## Results

Both models achieve high accuracy (>98%) on the MNIST test dataset.

## Technologies Used

- Python 3.x
- TensorFlow / Keras
- NumPy
- Matplotlib
- OpenCV
- PIL (Pillow)

## License

This project is open source and available for educational purposes.

## Author

BMDL Group - G14
