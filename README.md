# soilclassification_annam

This repository contains my individual solutions for the Annam Soil Image Classification challenges. The goal is to accurately classify soil types from images using deep learning.

---

## Project Overview

I developed a complete workflow for soil image classification, including data preparation, model training with transfer learning, prediction, and submission formatting. The project is organized for clarity and easy adaptation.

---

## Features

- **Flexible Data Handling:**  
  Works with both labeled (train/validation) and unlabeled (test) datasets. Handles column names such as `image_id` and `label` as required by the competition.

- **Modern Deep Learning Model:**  
  Utilizes EfficientNet-B3 with transfer learning for robust image feature extraction and classification.

- **Training Pipeline:**  
  Includes data augmentation, class imbalance handling, and validation monitoring to improve model performance.

- **Submission Ready:**  
  Generates predictions and formats the submission file exactly as required (`image_id,label`).

---

## Repository Structure

