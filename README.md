# Brain Tumor Detection Using Image Processing in MATLAB App Designer

## Overview

This project is a MATLAB GUI app (`.mlapp`) that performs basic brain tumor detection from MRI images using classical image processing techniques. Developed using **App Designer**, this app demonstrates the power of filters and segmentation in detecting potential tumor regions — all without the use of machine learning or deep learning.

> ⚠️ This project is for **educational/demo purposes** only and is **not intended for clinical diagnosis**.

---

## Features

- **Image Upload** — Select any `.jpg`, `.png`, or `.bmp` image
- **Median Filtering** — Reduces noise from MRI images
- **Edge Detection** — Highlights boundaries using the Sobel method
- **Tumor Region Detection** — Fills enclosed regions and highlights them in yellow
- **Multi-stage Image Display** — Shows all image stages side by side in the GUI

---

##  How to Run the App

1. Open MATLAB.
2. Navigate to the folder containing `brain.mlapp`.
3. Double-click `brain.mlapp` to open it in App Designer.
4. Click **Run** to launch the GUI.
5. Follow these steps in order:
   - Click **Upload Image**
   - Click **Median Filtering**
   - Click **Edge Detection**
   - Click **Tumor Detection**

Each processed image will be displayed in a separate panel for comparison.

---

##  Processing Pipeline

| Step | Description |
|------|-------------|
| 1. Upload Image | Supports JPG, PNG, BMP |
| 2. Median Filtering | Grayscale + `medfilt2()` |
| 3. Edge Detection | Sobel edge detection |
| 4. Tumor Detection | `imfill()` + segmentation logic |

Tumor regions are **highlighted in yellow** over the original image using pixel-wise masking.

---

## Requirements

- MATLAB R2019b or later
- Image Processing Toolbox
- App Designer Support (included in most MATLAB installations)

---

## Screenshots

### Original Image
![Original](image1.png)

### After Median Filtering
![Median Filter](image2.png)

### After Edge Detection
![Edge Detection](image3.png)

### Tumor Detection Result
![Tumor Detection](image4.png)



