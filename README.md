# Deep Denoising for Low-Dose X-rays

This repository contains three Jupyter notebooks implementing state-of-the-art deep learning architectures — DnCNN, ResUNet, and a hybrid of both — to denoise low-dose X-ray images while preserving diagnostic structures. These models aim to enhance image quality for improved clinical interpretation in resource-constrained medical environments.

---

## Overview

| Notebook Name       | Description |
|---------------------|-------------|
| `dncnn.ipynb`       | Implements the DnCNN architecture, a CNN-based approach for blind Gaussian denoising. |
| `resunet.ipynb`     | Implements the ResUNet architecture, combining U-Net with residual connections for improved structural preservation. |
| `hybrid-denoiser.ipynb` | Combines DnCNN and ResUNet features for enhanced denoising, leveraging the strengths of both models. |

---

## Motivation

Low-dose X-ray imaging is essential to reduce patient radiation exposure, especially in pediatric and routine screenings. However, lower doses introduce significant noise, which can obscure critical anatomical features. This project focuses on leveraging deep learning to:

- **Remove noise**
- **Preserve diagnostic detail**
- **Support safer medical imaging workflows**

---

## Dataset

The models were trained and evaluated on publicly available datasets, such as:

- **NIH Chest X-rays** and
- **Pediatric Pneumonia Dataset**

Noise augmentation techniques were applied to simulate the effects of low-dose acquisition.

---

## Results & Evaluation

Evaluation metrics include:

- **PSNR** (Peak Signal-to-Noise Ratio)
- **SSIM** (Structural Similarity Index)

---

## References

1. Zhang et al., *“Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising”*, CVPR 2017.
2. Ronneberger et al., *“U-Net: Convolutional Networks for Biomedical Image Segmentation”*, MICCAI 2015.
