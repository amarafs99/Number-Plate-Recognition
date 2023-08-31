# License Plate Detection and Recognition

This repository contains a Python script for detecting and recognizing license plates in an image using the EasyOCR library and OpenCV.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Loading and Preprocessing an Image](#loading-and-preprocessing-an-image)
  - [Reducing Noise and Edge Detection](#reducing-noise-and-edge-detection)
  - [Applying Thresholding and Finding Contours](#applying-thresholding-and-finding-contours)
  - [Masking the License Plate](#masking-the-license-plate)
  - [Recognizing the License Plate](#recognizing-the-license-plate)
- [Results](#results)
- [Contributions](#contributions)
- [License](#license)

## Introduction

This code demonstrates how to detect and recognize license plates in an image using the EasyOCR library for optical character recognition and OpenCV for image processing.

## Getting Started

### Prerequisites

- Python 3.x
- OpenCV
- Matplotlib
- NumPy
- EasyOCR

### Installation

1. Clone this repository:
git clone https://github.com/AbhiD98/license-plate-recognition.git


## Usage

### Loading and Preprocessing an Image

The script loads an image in this case ('1.jpg') and converts it to grayscale. The original and grayscale images are displayed using Matplotlib.

### Reducing Noise and Edge Detection

Non-Local Means Denoising is applied to reduce noise, and edge detection is performed using the Canny edge detection algorithm. The denoised and edge images are displayed.

### Applying Thresholding and Finding Contours

Thresholding is applied to create a binary image, and contours are detected using OpenCV. The script sorts the contours by area and draws the top 3 contours on a copy of the original image.

### Masking the License Plate

The largest contour is assumed to correspond to the license plate. The script creates a mask and uses it to extract the license plate region from the original image.

### Recognizing the License Plate

The EasyOCR library is used to recognize text from the license plate image. The extracted license plate text is printed.

## Results

The results of the license plate detection and recognition process are displayed in the console. The recognized license plate text provides information about the detected license plate.

## Contributions

Contributions to this repository are welcome! If you find any issues or have improvements to suggest, please feel free to create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
