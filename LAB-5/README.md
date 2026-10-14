# Lab 5 — Spatial Filtering: Smoothing and Sharpening

**Course:** ARTI 403 — Image Processing

## Overview

This lab explores spatial filtering techniques for image smoothing and sharpening using Python, OpenCV, NumPy, and Matplotlib.

## Tasks

### Task 1: 7×7 Box Filter

Apply a 7×7 box filter to smooth an image, then display the original and smoothed images side by side.

### Task 2: Gaussian Filtering

Apply 5×5 and 21×21 Gaussian filters to an image. Display the original image and both filtered results side by side to compare their smoothing effects.

### Task 3: Laplacian Sharpening

Apply a 3×3 Laplacian filter and sharpen the image using the following formula:

```python
np.clip(image_float - laplacian, 0, 1)
```

Display the original image, the Laplacian response, and the sharpened image.

## Requirements

- Python 3
- OpenCV (`opencv-python`)
- NumPy
- Matplotlib
- Jupyter Notebook or JupyterLab

Install the required packages:

```bash
pip install opencv-python numpy matplotlib notebook
```

## Project Structure

```text
Lab5/
├── README.md
├── lab5.ipynb
└── images/
    └── parrot.png
```

The notebook expects the image at `images/Parrot.png` by default. To use another image, update the `image_path` variable in the notebook.

## How to Run

1. Clone or download the repository.
2. Ensure the image is available at the path specified by `image_path`.
3. Install the required packages.
4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `lab5.ipynb`.
6. Run all cells from top to bottom.

## Expected Results

- **Box Filter:** A smoothed image using a 7×7 averaging kernel.
- **Gaussian Filtering:** Two smoothed images using 5×5 and 21×21 kernels. The larger kernel generally produces stronger blur.
- **Laplacian Sharpening:** The Laplacian response and a sharpened version of the original image.

Results depend on the input image.

## References

- [OpenCV — Image Filtering](https://docs.opencv.org/4.x/d4/d13/tutorial_py_filtering.html)
- [Data Carpentry — Blurring](https://datacarpentry.github.io/image-processing/06-blurring.html)
