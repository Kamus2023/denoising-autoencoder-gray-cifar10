# Denoising Autoencoder for Grayscale CIFAR-10

This project implements a lightweight U-Net-style convolutional autoencoder with skip connections for Gaussian noise removal on grayscale CIFAR-10 images.

## 🧠 Highlights
- Trained on a tiny dataset (100 grayscale images) with 64x64 resolution.
- Achieves PSNR > 27 dB, SSIM > 0.8, and MSE < 0.002 on test set.
- Employs a hybrid loss (MSE + SSIM) to preserve both pixel and structure fidelity.
- Robust to varying noise levels (σ ∈ [0.1, 0.4]).

## 📁 Folder Structure
- `notebooks/`: Main notebook for model training and evaluation.
- `models/`: Optional structure figures.
- `images/`: Sample visual results.
- `requirements.txt`: Python dependencies.

## 🚀 Quick Start
```bash
# Install dependencies
pip install -r requirements.txt

# Open notebook
jupyter notebook notebooks/denoising_autoencoder.ipynb
