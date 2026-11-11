# Lab 9 – Morphological Operations

## Overview

This project demonstrates morphological image processing techniques using Python and OpenCV.

The objective is to apply erosion, dilation, opening, and closing to binary images and investigate how different structuring element shapes and sizes affect the processed results.

## Project Structure

```text
Lab9/
│
├── Lab 9_Morphological_Operations.ipynb
├── README.md
│
└── images/
    ├── Erosion2.jpg
    ├── Open_Closing.jpg
    ├── Opening2.jpg
    ├── BoundaryExtraction.jpg
    └── Balls.png
```

## Requirements

- Python 3
- Jupyter Notebook
- OpenCV
- NumPy
- Matplotlib

## Installation

Install the required libraries using:

```bash
pip install numpy opencv-python matplotlib notebook nbconvert
```

## Running the Notebook

1. Place all required images inside the `images` folder.
2. Open the notebook using Jupyter Notebook.
3. Run all cells in order.
4. Review the generated morphological operation results.

## Tasks

### Task 1 – Morphological Operations

Apply the following operations to a new binary image:

- Erosion
- Dilation
- Opening
- Closing

Display the original binary image alongside the processed results.

### Task 2 – Structuring Element Comparison

Compare three structuring element shapes:

- Square
- Cross
- Ellipse

Experiment with the following kernel sizes:

- 3×3
- 5×5
- 7×7

Apply both erosion and dilation and compare the resulting images.

## Boundary Extraction

The notebook also demonstrates:

- Morphological Gradient
- Internal Boundary Extraction
- External Boundary Extraction

## Output

The notebook generates visual comparisons showing how morphological operations, structuring element shapes, and kernel sizes affect binary images.
