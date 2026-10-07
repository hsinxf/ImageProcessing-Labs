# ARTI 404 – Image Processing

## Lab 4: Intensity Transformations and Filtering – Spatial Domain

### Overview

This lab focuses on fundamental image processing techniques using Python. The lab covers thresholding, histogram processing, contrast stretching, histogram equalization, and histogram matching.

### Tools and Libraries

- Python 3
- Jupyter Notebook
- OpenCV
- NumPy
- Matplotlib
- scikit-image

### Project Structure

```text
Lab4/
│
├── Lab4.ipynb
│
├── README.md
│
└── images/
    └── Parrot.png
```

### Task 1: Thresholding

A grayscale image is loaded using OpenCV and thresholding is applied using different threshold values:

- 0
- 50
- 100
- 150
- 200

The thresholding operation converts the grayscale image into a binary image, separating foreground and background based on pixel intensity.

**Image used:** `images/Parrot.png`

### Task 2: Histogram Processing

The built-in `moon` image from `skimage.data` is used for histogram processing.

#### Contrast Stretching

The intensity values are rescaled using the 2nd and 98th percentiles. The original image and its histogram are compared with the contrast-stretched image and histogram.

### Assessment Task 1: Contrast Stretching

The `moon` image is processed using the 3rd and 80th percentiles. The resulting image and its histogram are displayed.

### Assessment Task 2: Histogram Equalization

Histogram equalization is applied to the `moon` image using:

```python
exposure.equalize_hist()
```

The equalized image and its histogram are displayed to show how the intensity distribution changes.

### Assessment Task 3: Histogram Matching

Histogram matching is performed using two images provided by `skimage.data`:

- **Rocket** – reference image
- **Chelsea** – source image

The histogram of the Chelsea image is matched to the histogram of the Rocket image. The original images, matched result, and histograms are displayed.

### Images

The only external image required for this lab is:

```text
images/Parrot.png
```

The `moon`, `rocket`, and `chelsea` images are loaded directly from `skimage.data`, so they do not need to be downloaded separately.

### How to Run

1. Open `Lab4.ipynb` using Jupyter Notebook.
2. Make sure `Parrot.png` is inside the `images` folder.
3. Run the cells from top to bottom.
4. Check that all images, thresholding results, and histograms are displayed correctly.

### Submission

The final folder should contain:

- The completed Jupyter Notebook
- `README.md`
- The required image(s) used in the lab

### Course

**Course:** ARTI 404 – Image Processing
**Lab:** 4
**Topic:** Intensity Transformations and Filtering – Spatial Domain
