# ARTI 404 – Image Processing

## Lab 3 – Image Manipulations using OpenCV

This repository contains the implementation of Lab 3 for the ARTI 404 – Image Processing course.

The lab focuses on reading, manipulating, and transforming digital images using Python and the OpenCV library.

## Tools and Libraries

- Python 3
- Jupyter Notebook
- OpenCV (`cv2`)
- NumPy
- Matplotlib

## Project Structure

```text
Lab3/
│
├── Lab3.ipynb
├── README.md
│
└── images/
    ├── input.jpg
    ├── original.jpg
    ├── resized.jpg
    ├── rotated_120.jpg
    ├── sheared.jpg
    ├── grayscale.jpg
    ├── negative.jpg
    ├── log_transformation.jpg
    └── power_law.jpg
```

## Lab Tasks

### Task 1 – Geometric Transformations

The following geometric transformations are applied to the input image:

1. Increase the size of the image.
2. Rotate the image by 120 degrees.
3. Perform a shear transformation.

### Task 2 – Intensity Transformations

The following intensity transformations are applied to the image:

1. Convert the image to grayscale.
2. Create a negative image.
3. Apply logarithmic transformation.
4. Apply power-law transformation.

For the power-law transformation, a gamma value of `0.5` is used.

## Input Image

The original image used in this experiment is stored in:

```text
images/input.jpg
```

## Output Images

The processed images are saved in the `images` folder:

- `resized.jpg` – Increased image size.
- `rotated_120.jpg` – Image rotated by 120 degrees.
- `sheared.jpg` – Sheared image.
- `grayscale.jpg` – Grayscale version.
- `negative.jpg` – Negative transformation.
- `log_transformation.jpg` – Logarithmic transformation.
- `power_law.jpg` – Power-law transformation.

## How to Run

1. Open `Lab3.ipynb` using Jupyter Notebook.
2. Make sure the `images` folder is in the same directory as the notebook.
3. Make sure `input.jpg` is inside the `images` folder.
4. Run the notebook cells from top to bottom.
5. The generated results will be saved inside the `images` folder.

## Image Path

Since the images are stored inside the `images` folder, the input image is loaded using:

```python
img = cv2.imread('images/input.jpg')
```

## Conclusion

This lab demonstrates basic image manipulation techniques using OpenCV. Geometric transformations such as resizing, rotation, and shearing were performed, followed by intensity transformations including grayscale conversion, negative transformation, logarithmic transformation, and power-law transformation.
