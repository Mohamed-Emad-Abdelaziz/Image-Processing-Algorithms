# Image-Processing-Algorithms

![Project Image]([https://example.com/your-image.png](https://files.oaiusercontent.com/file-XjJTuiR5DD5of2o5kDMG1h?se=2025-02-17T20%3A07%3A41Z&sp=r&sv=2024-08-04&sr=b&rscc=max-age%3D604800%2C%20immutable%2C%20private&rscd=attachment%3B%20filename%3D112f1999-6cc7-4dbe-83cb-40d5918173af.webp&sig=Ouiv6oZMdvj%2BKsW%2BS3cYmKZoU/y1uQ8t36GsRfh3FAQ%3D))

## Overview

This project applies various image processing filters and transformations using different algorithms. A simple GUI built with Tkinter allows users to easily select an image and apply filters.

## Team Members

| Name             | ID     |
| ---------------- | ------ |
| Sherif Mohammed  | 213485 |
| Mohamed Emad     | 213411 |
| Yousef Amr       | 212473 |

## Features

### Graphical User Interface (GUI)
- Built using Tkinter.
- Simple interface with buttons to select an image and apply filters.

### Filters

#### Smoothing (Spatial Filters)
- **Median Filter**
- **Adaptive Filter (Max)**
- **Averaging Filter**
- **Gaussian Filter:**  
  Generates a 5x5 kernel for each cell and applies it to the image.

#### Sharpening (Spatial Filters)
- **Laplacian Operator:**  
  Uses a 5x5 kernel for better results:
  - **Unsharp Masking and Highboost Filtering:**  
Blurs the image using a Gaussian filter, subtracts the blurred image to create a mask, then applies a filter based on the user-defined parameter to select between highboost filtering or unsharp masking.
- **Roberts Cross-Gradient Operators**
- **Sobel Operators**

#### Noise Filters
- **Impulse Noise (Salt and Pepper)**
- **Gaussian Noise**
- **Uniform Noise**

#### Transform / Frequency Domain Filters
- **Histogram Equalization:**  
Calculates the recurrence of each intensity value, computes the probability by multiplying by the image dimensions, and maps new intensity values.
- **Histogram Specification:**  
Similar to equalization but uses a reference image to match the histogram.
- **Fourier Transform (Forward and Inverse):**  
Uses multi-threading and vectorized calculations for speed, and shifts the low-frequency components to the center for visualization.
- **Interpolation (Nearest Neighbor):**  
Resizes the image based on a user-provided scale factor by mapping the coordinates accordingly.

## Getting Started

1. **Clone the Repository:**
 ```bash
 git clone https://github.com/YourUsername/YourRepo.git

