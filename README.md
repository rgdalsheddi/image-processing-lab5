# image-processing-lab5
# Spatial Filtering: Smoothing and Sharpening

A computer vision lab demonstrating different spatial filtering techniques for image smoothing, noise reduction, edge preservation, and sharpening using Python and OpenCV.

The notebook explores how different filters modify image pixels based on their surrounding neighborhood and compares their effects on image quality and detail preservation.

## Features

This lab implements and compares several spatial filtering techniques:

- Unsharp Masking
- 7×7 Box Filtering
- Gaussian Filtering with different kernel sizes
- Laplacian Sharpening
- Median Filtering
- Bilateral Filtering
- Salt-and-Pepper Noise Reduction
- Comparison of different smoothing kernel sizes

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-image
- Jupyter Notebook

## Filtering Techniques

### 1. Unsharp Masking

Unsharp masking improves image sharpness by:

1. Creating a blurred version of the image.
2. Calculating the difference between the original and blurred image.
3. Adding the difference back to the original image.

This enhances edges and fine details.

---

### 2. Box Filter

A box filter replaces each pixel with the average value of neighboring pixels.

A manually created **7×7 kernel** is applied using:

```python
cv2.filter2D()
