# Visualizing-DCT-in-python

# **DCT-Based Image Compression**

This repository demonstrates **Discrete Cosine Transform (DCT)**-based image compression, similar to the JPEG standard, using Python. The project walks you through the entire process, from loading an image to applying DCT, quantization, and reconstructing the image. It includes visualizations and comparisons to help you understand the effects of compression.

---

## **Table of Contents**
1. [Introduction](#introduction)
2. [Steps](#steps)
3. [Results](#results)
4. [Dependencies](#dependencies)
5. [References](#references)

---

## **Introduction**
The **Discrete Cosine Transform (DCT)** is a key component of image compression algorithms like JPEG. It converts spatial image data into frequency components, allowing for efficient compression by discarding less perceptually important information. This project demonstrates how DCT works, how quantization affects image quality, and how to reconstruct the compressed image.

---

## **Steps**
1. **Import Libraries**: Use Python libraries like `numpy`, `scipy`, `matplotlib`, and `PIL` for image processing and visualization.
2. **Load and Preprocess the Image**: Upload an image, convert it to grayscale, and resize it for easier computation.
3. **Apply DCT to 8x8 Blocks**: Divide the image into 8x8 blocks and apply 2D DCT to each block.
4. **Quantization**: Use a standard JPEG quantization matrix to reduce the precision of DCT coefficients.
5. **Reconstruct the Image**: Dequantize the coefficients, apply inverse DCT, and combine the blocks back into an image.
6. **Visualize Results**: Compare the original and reconstructed images and calculate the Mean Squared Error (MSE).

---

## **Results**
- **Original vs. Reconstructed Image**: The reconstructed image will look similar to the original but may have slight artifacts (blocking, blurring) due to quantization.
- **Mean Squared Error (MSE)**: A measure of the difference between the original and reconstructed images. Lower values indicate better quality.

---

## **Dependencies**
- Python 3.x
- Libraries:
  - `numpy`
  - `scipy`
  - `matplotlib`
  - `PIL` (Pillow)

---

## **References**
- [JPEG Standard (Annex A)](https://www.w3.org/Graphics/JPEG/itu-t81.pdf)
- [3Blue1Brown’s Fourier Transform Video](https://www.youtube.com/watch?v=spUNpyF58BY)
- [Scipy Documentation](https://docs.scipy.org/doc/scipy/reference/fftpack.html)

---
