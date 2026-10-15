# ARTI403 – Lab 6: Frequency Domain

## Overview

This lab focuses on filtering in the frequency domain using Python and the Fast Fourier Transform (FFT).

## Objective

Implement fundamental image processing algorithms in the frequency domain.

## Requirements

- Python 3
- NumPy
- Matplotlib
- Scikit-image

## Task 1: Filtering in the Frequency Domain

### Part 1: Laplacian Filtering

- Load the Cameraman grayscale image.
- Resize the image to 256 × 256 pixels.
- Apply the 2D FFT to the image.
- Implement the Laplacian filter in the frequency domain.
- Apply the filter and use the inverse FFT to obtain the spatial output.
- Display the original image, Laplacian spectrum, and filtered result.

### Assessment: Sobel Filtering

- Use the same Cameraman image.
- Apply Sobel X and Sobel Y filters in the frequency domain.
- Display the filtering results.

## How to Run

1. Open `lab6.ipynb` in Jupyter Notebook or Visual Studio Code.
2. Install the required libraries if necessary:

   ```bash
   python -m pip install numpy matplotlib scikit-image
   ```

3. Run all notebook cells in order.

## Image

The notebook uses the Cameraman image provided by `skimage.data.camera()`. No separate image file is required.

## Submission

- `lab6.ipynb`
- `lab6.pdf`
- `README.md`

Submit the GitHub repository link through Blackboard, as instructed in the lab manual.

## Conclusion

This lab demonstrates frequency-domain image filtering using the FFT. The Laplacian filter emphasizes intensity changes, while the Sobel filters detect edges in different directions.
