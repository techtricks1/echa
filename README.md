# Handwritten Digit Recognition using Transfer Learning

## Overview

This project implements handwritten digit recognition using transfer learning with the VGG16 model. The goal is to leverage pre-trained convolutional layers from VGG16 and train a custom top model for recognizing digits.

## Key Components

- **Data Preprocessing:**
  - Grayscale images from the MNIST dataset are resized and converted to RGB format.
  - Images are normalized to a range of [0, 1].

- **Model Architecture:**
  - VGG16 model with frozen convolutional layers.
  - Custom top model for digit recognition.

- **Model Training:**
  - Compiled using the Adam optimizer and categorical crossentropy loss.
  - Trained on the preprocessed MNIST dataset for one epoch.

- **Drawing and Recognition:**
  - Interactive drawing and recognition with the `draw_and_recognize` function.

- **Evaluation and Visualization:**
  - Model accuracy on the test set.
  - Confusion matrix visualization.

## Usage

To use the interactive drawing and recognition feature, call the `draw_and_recognize` function with your trained model.

```python
# Call the function with your trained model
draw_and_recognize(model)
