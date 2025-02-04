# epilepsy-classification-using-data-from-Bonn-university
# Overview
This project implements an epilepsy classification system using EEG data from the Bonn University dataset. The approach follows a research-based methodology that combines Continuous Wavelet Transform (CWT), a Convolutional Autoencoder (CAE), and Principal Component Analysis (PCA) to extract and classify meaningful features from EEG signals.

# Dataset
The Bonn University EEG dataset consists of five classes:

Z (Healthy)
O (Healthy with open eyes)
N (Interictal - Epilepsy-free)
F (Pre-ictal - Near seizure onset)
S (Ictal - Seizure state)
Each class contains 100 samples, digitized at 173.61 Hz with 4097 time points per sample.

# Methodology
Preprocessing:

Normalized EEG signals
Applied Continuous Wavelet Transform (CWT) with a window size of 1458 and an overlap of 486
Generated scalogram images (size: 50 × 1458 × 1)
Feature Extraction:

Used a Convolutional Autoencoder (CAE) to learn latent representations
Applied PCA to reduce the latent space to 128 dimensions
Extracted statistical features for a hybrid feature set
Classification:

Trained machine learning models using the hybrid feature set
Evaluated performance using standard metrics
# Results
The combination of CWT + Autoencoder + PCA + Statistical Features enhances classification performance by capturing both time-frequency and statistical characteristics of EEG signals.
