# Lab 8 - Edge Detection

## Overview
This notebook applies and compares edge detection methods using Python, NumPy, Matplotlib, and OpenCV. It includes Sobel, Roberts, Prewitt, Canny, multi-channel Canny, LoG, DoG, and color-gradient examples. It also completes the required Canny threshold comparison.

## Folder structure

Keep the notebook and the `image` folder in the same directory:

```text
Lab_8_Edge_Detection(1).ipynb
README.md
image/
    kid1.jpg
    butterfly.jpg
    bird.jpg
    coins.jpg
```

The notebook initially loads `image/kid1.jpg`. If your file has a different name or extension, edit `imgFile` in the first code cell. For example:

```python
imgFile = "image/butterfly.jpg"
```

The image files are not embedded in the notebook; add your own images to the `image` folder before running it.

## Requirements

Install the required packages:

```bash
python -m pip install opencv-python numpy matplotlib jupyter nbconvert
```

## Run the notebook

From the directory containing the notebook:

```bash
jupyter notebook
```

Open `Lab_8_Edge_Detection(1).ipynb` and choose **Run All**.

## Convert the notebook to HTML

Run this command in the terminal:

```bash
jupyter nbconvert --to html --execute "Lab_8_Edge_Detection(1).ipynb" --output "Lab_8_Edge_Detection.html"
```

This executes the notebook and saves an HTML version with the results and plots. Make sure the `image` folder and selected image exist before running the command.

To convert an already executed notebook without executing it again:

```bash
jupyter nbconvert --to html "Lab_8_Edge_Detection(1).ipynb" --output "Lab_8_Edge_Detection.html"
```

## Save as PDF

1. Open `Lab_8_Edge_Detection.html` in Chrome or Microsoft Edge.
2. Press `Ctrl + P` (Windows/Linux) or `Cmd + P` (macOS).
3. Set the destination/printer to **Save as PDF**.
4. Save the PDF.

## Required Canny threshold experiment

The notebook compares these threshold pairs on the same image:

- Low = 30, High = 90
- Low = 50, High = 150
- Low = 100, High = 200

In general, lower thresholds retain more weak edges and fine details but may also detect more noise. Higher thresholds suppress weak edges, producing fewer and stronger edges while potentially removing small details. The actual result depends on the image.
