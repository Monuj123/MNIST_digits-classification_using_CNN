
# MNIST Digit Classification using CNN

## Overview
This project implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset. The model achieves **98.87% accuracy** on the test set, demonstrating the effectiveness of CNNs for image classification tasks.

## Dataset
The **MNIST dataset** (Modified National Institute of Standards and Technology) consists of:
- **60,000** training images of handwritten digits (0-9)
- **10,000** test images
- Each image is **28×28 pixels** in grayscale

## Model Architecture

| Layer Type | Output Shape | Parameters |
|------------|--------------|------------|
| Conv2D (32 filters, 3×3) | 26×26×32 | 320 |
| MaxPooling2D (2×2) | 13×13×32 | 0 |
| Conv2D (64 filters, 3×3) | 11×11×64 | 18,496 |
| MaxPooling2D (2×2) | 5×5×64 | 0 |
| Flatten | 1600 | 0 |
| Dense (10 units, softmax) | 10 | 16,010 |

**Total Parameters:** 34,826 (136 KB)

## Requirements

```bash
tensorflow>=2.0.0
numpy>=1.19.0
matplotlib>=3.3.0
scikit-learn>=0.24.0
