# soilclassification_annam

This repository contains my individual solutions for the Annam Soil Image Classification challenges. The goal is to accurately classify soil types and detect soil presence in images using deep learning.

---

## Project Overview

I developed a complete workflow for soil image classification, including data preparation, model training with transfer learning and autoencoders, prediction, and submission formatting. The project is organized for clarity and easy adaptation.

---

## Features

- **Flexible Data Handling:**  
  Supports both labeled (train/validation) and unlabeled (test) datasets. Handles competition-specific CSV formats with columns like `image_id` and `label`.

- **Modern Deep Learning Models:**  
  - **Challenge 1:** EfficientNet-B3 with transfer learning for robust multi-class soil type classification.  
  - **Challenge 2:** One-class convolutional autoencoder for soil vs. not-soil detection.

- **Training Pipeline:**  
  Includes data augmentation, class imbalance handling, stratified splitting, and validation monitoring.

- **Submission Ready:**  
  Generates predictions and formats the submission file as required (`image_id,label`).

---

## Challenge 1: Soil Type Classification

### Task  
Classify each image into its correct soil type (e.g., clay, loam, sand, etc.).

### Approach  
- Pre-trained EfficientNet-B3 model fine-tuned on soil images.  
- Extensive data augmentation and normalization.  
- Labels encoded numerically.  
- Training/validation split for monitoring.  
- Model selection based on validation F1-score.


---

## Challenge 2: Soil vs. Not-Soil Detection

### Task  
Determine whether an image contains soil or not, using only soil images for training.

### Approach  
- Convolutional autoencoder trained to reconstruct soil images.  
- Mean squared error (MSE) loss for training.  
- Reconstruction error threshold (e.g., 99th percentile) for prediction.  
- Binary predictions formatted for submission.



