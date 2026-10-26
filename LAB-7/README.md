# Lab 7 — Color Image Processing

This folder contains the color-image versions of the two Lab 7 notebooks:

- `Lab_7_A_Laplacian_Filter_Color_Checked.ipynb` — Laplacian edge response and sharpening.
- `Lab_7_B_Maths_Statistics_Filters_Color_Checked.ipynb` — noise generation and mathematical/statistical filters.

## Requirements

Python 3.9+ is recommended. The notebooks use:

- OpenCV (`opencv-python`)
- NumPy
- Matplotlib
- Jupyter

Install dependencies from a terminal:

```bash
python3 -m pip install opencv-python numpy matplotlib notebook nbconvert
```

## Input image

Both notebooks load this relative path:

```text
images/parrot.png
```

Create an `images` folder beside the notebooks and put a color image named `parrot.png` inside it. Alternatively, edit `imgFile` in Lab 7(A) or `imgPath` in Lab 7(B) to point to your image.

OpenCV reads images in BGR order, so the notebooks convert the image to RGB before displaying it with Matplotlib.

## Run the notebooks

From the directory containing the notebooks:

```bash
jupyter notebook
```

Open each notebook and choose **Kernel → Restart Kernel and Run All Cells**.

## Convert `.ipynb` to PDF from the terminal

### Option 1 — Direct PDF export (requires a working LaTeX installation)

```bash
jupyter nbconvert --to pdf "Lab_7_A_Laplacian_Filter_Color_Checked.ipynb"
jupyter nbconvert --to pdf "Lab_7_B_Maths_Statistics_Filters_Color_Checked.ipynb"
```

On macOS, a common LaTeX option is MacTeX. On Ubuntu/Debian, install a TeX distribution such as `texlive-xetex` and any missing LaTeX packages if nbconvert reports errors.

### Option 2 — HTML, then print to PDF (no LaTeX required)

First export to HTML:

```bash
jupyter nbconvert --to html "Lab_7_A_Laplacian_Filter_Color_Checked.ipynb"
jupyter nbconvert --to html "Lab_7_B_Maths_Statistics_Filters_Color_Checked.ipynb"
```

Then open the generated `.html` files in a browser and choose **Print → Save as PDF**.

### Option 3 — WebPDF (requires Playwright/Chromium)

Install the WebPDF support:

```bash
python3 -m pip install "nbconvert[webpdf]"
python3 -m playwright install chromium
```

Then convert:

```bash
jupyter nbconvert --to webpdf --allow-chromium-download "Lab_7_A_Laplacian_Filter_Color_Checked.ipynb"
jupyter nbconvert --to webpdf --allow-chromium-download "Lab_7_B_Maths_Statistics_Filters_Color_Checked.ipynb"
```

## Notes

- Run all cells before exporting if you want the output images included in the PDF.
- If the notebooks are exported without executing cells, their previous saved outputs may be used.
- If a notebook fails because the image path is wrong, fix the path or place the image in `images/parrot.png`.
