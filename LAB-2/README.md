# Lab 2 – Digital Image Fundamentals

## Course Information

- **Course:** ARTI 403 – Image Processing
- **Lab:** Lab 2
- **Topic:** Digital Image Fundamentals
- **Programming Language:** Python
- **Tools:** Jupyter Notebook, OpenCV, NumPy, Pillow

---

## Introduction

This lab introduces basic digital image processing concepts, including image sampling, image quantization, arithmetic operations, and set/logical operations on images.

The practical tasks are implemented using Python and image processing libraries.

---

## Project Structure

```text
Lab2/
│
├── Lab2.ipynb
├── README.md
│
└── images/
    ├── lena_gray_256.tif
    ├── cameraman.tif
    ├── A.png
    └── B.png
```

---

## Task 1 – Sampling and Quantization

In this task, the image `lena_gray_256.tif` is loaded as a grayscale image.

### Sampling

Sampling is performed by reducing the spatial resolution of the image using a sampling factor.

The sampling factor can be changed to observe its effect on the image quality.

### Quantization

Quantization reduces the number of intensity levels in an image.

Different quantization levels are tested to observe their effect on the image.

### Parameters Used

Initial parameters:

- Sampling factor: **14**
- Quantization levels: **9**

Additional values were tested to observe the changes in image quality.

---

## Task 2 – Arithmetic Operations

Two grayscale images are used:

- `lena_gray_256.tif`
- `cameraman.tif`

The images are resized to the same dimensions before performing arithmetic operations.

### 1. Image Subtraction

The two images are subtracted to produce a difference image.

### 2. Adding a Constant

A constant value of **175** is added to one of the images.

This increases the intensity values of the image, with values above 255 limited to the valid grayscale range.

---

## Set and Logical Operations

Two grayscale images are used:

- `A.png`
- `B.png`

The following operations are performed:

### 3. Set Difference

The set difference between image A and image B is calculated.

### 4. Symmetric Difference

The symmetric difference is calculated using the XOR operation.

### 5. Intersection

The intersection of the two images is calculated using the AND operation.

### 6. Union

The union operation is also demonstrated using the OR operation.

---

## Libraries Used

The following Python libraries are used:

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
from PIL import Image
```

---

## Results

The notebook displays the results of:

- Original image
- Sampled images
- Quantized images
- Image subtraction
- Image + 175
- Set difference
- Symmetric difference
- Intersection
- Union

The results can be observed directly in `Lab2.ipynb`.

---

## Conclusion

In this lab, basic digital image processing operations were implemented using Python. The effects of sampling and quantization were observed by changing their parameters.

Arithmetic operations such as subtraction and addition with a constant were also performed. In addition, logical and set operations including difference, symmetric difference, intersection, and union were applied to
grayscale images.

These operations demonstrate how image intensity and spatial information can be manipulated using digital image processing techniques.
