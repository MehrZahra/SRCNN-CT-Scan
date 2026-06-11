# SRCNN-CT-Scan
Deep learning-based SRCNN model for enhancing CT scan images of rock sample

## Overview
This project implements a **Super-Resolution Convolutional Neural Network (SRCNN)** to enhance low-resolution CT scan images of rock samples**. The model learns to reconstruct high-resolution images from low-resolution inputs while preserving fine structural details such as pores, edges, and textures.

The implementation is developed using **PyTorch** and includes a full pipeline for data loading, training, evaluation, and visualization of results.

---

## Objective
- Enhance low-resolution CT scan images (LR → HR)
- Preserve geological structures (pores, fractures, textures)
- Improve image quality for rock analysis

---

## Model Architecture
- Conv Layer 1 (5×5, 64 filters)
- BatchNorm + ReLU
- Conv Layer 2 (5×5, 64 filters)
- BatchNorm + ReLU
- Bicubic Upsampling (×2)
- Final Conv Layer (1 channel output)

---

## Training
- Framework: PyTorch
- Loss: MSE
- Optimizer: Adam
- LR: 1e-6
- Epochs: 80

---

## Metrics
- PSNR
- SSIM

---

## Dataset
CT scan images of rocks (LR & HR pairs)

---

## Author
Zahra Mehrfar
