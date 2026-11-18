# Lab 10 — Image Segmentation and Feature Extraction

**Course:** ARTI404 — Image Processing  
**Institution:** Imam Abdulrahman Bin Faisal University

## Overview

This Jupyter notebook covers image segmentation and feature extraction using Python and OpenCV:

- **Canny Edge Detection:** detects edges in a grayscale image.
- **Harris Corner Detection:** detects corners in a checkerboard image.
- **Global Binary Thresholding:** segments an image using a fixed threshold (`T = 127`).
- **Q1 — Otsu's Thresholding (Solved):** automatically calculates the threshold and displays the original image, intensity histogram, and thresholded image.

The notebook also contains a summary table of common image-processing techniques.

## Files

- `Lab10_Image_Segmentation_Feature_Extraction_Solved.ipynb` — completed notebook, including Q1.
- `Lab10_Image_Segmentation_Feature_Extraction_Solved.html` — HTML export (generated using the steps below).

## Requirements

- Python 3
- Jupyter Notebook / JupyterLab and `nbconvert`
- `opencv-python`, `numpy`, `matplotlib`, `scikit-image`

If these packages are not already installed:

```bash
python3 -m pip install notebook nbconvert opencv-python numpy matplotlib scikit-image
```

## Convert the notebook to HTML on macOS

Open **Terminal**, navigate to the folder containing the solved notebook, and run:

```bash
cd ~/Downloads
jupyter nbconvert --to html "Lab10_Image_Segmentation_Feature_Extraction_Solved.ipynb"
open "Lab10_Image_Segmentation_Feature_Extraction_Solved.html"
```

> Replace `~/Downloads` with your folder if the notebook is stored elsewhere. This basic export includes **existing saved outputs**; it does not rerun cells.

### Optional: Execute all cells and then export

To generate fresh plots and results before exporting, run:

```bash
cd ~/Downloads
jupyter nbconvert --execute --to html \
  "Lab10_Image_Segmentation_Feature_Extraction_Solved.ipynb" \
  --ExecutePreprocessor.timeout=120
open "Lab10_Image_Segmentation_Feature_Extraction_Solved.html"
```

Execution requires the dependencies above to be installed in the notebook's Python environment. If `jupyter` is not found, try `python3 -m jupyter nbconvert` after installing Jupyter in that environment.

## Expected Q1 Result

Otsu's method uses `cv2.THRESH_OTSU` to automatically compute a threshold for the sample `skimage.data.coins()` image. The output includes:

1. The original grayscale image.
2. A pixel-intensity histogram with the chosen threshold marked.
3. The binary thresholded image.

## Notes

- Run the notebook cells in order if using Jupyter interactively.
- No external image files are needed; sample images come from `skimage.data`.
- The HTML file can be opened locally in a browser and shared without requiring Jupyter to view it.
