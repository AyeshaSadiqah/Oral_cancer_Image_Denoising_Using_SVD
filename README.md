# Oral_cancer_Image_Denoising_Using_SVD
This repository presents a classical image denoising approach using **Singular Value Decomposition (SVD)** on a dataset of oral cancer and non-cancer images. It demonstrates how SVD can effectively reduce noise and enhance image clarity in medical image preprocessing.

## 📌 Objective

- Apply SVD-based image denoising to oral cancer images.
- Measure denoising effectiveness using image quality metrics.
- Visualize the differences between original, noisy, and denoised images.
- Demonstrate a simple and interpretable denoising pipeline.

## 🗂 Dataset

The dataset  contains two classes:

- `CANCER`: Images of diagnosed oral cancer.
- `NON CANCER`: Images of non-cancerous cases.

All images are:
- Resized to `32x32` pixels.
- Converted to tensor format using `torchvision.transforms`.

## 🧪 Methodology

1. **Image Loading**
   - Loads and resizes oral cancer images from two categories.

2. **Noise Addition**
   - Adds Gaussian noise to simulate real-world degradation.

3. **SVD Denoising**
   - Applies SVD to decompose each image matrix.
   - Truncates smaller singular values to reconstruct denoised images.

4. **Evaluation Metrics**
   - **PSNR** (Peak Signal-to-Noise Ratio)
   - **MSE** (Mean Squared Error)
   - **SSIM** (Structural Similarity Index)

5. **Visualization**
   - Displays original, noisy, and denoised images side-by-side for qualitative assessment.
