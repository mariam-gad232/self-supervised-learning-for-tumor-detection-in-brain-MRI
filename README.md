# self-supervised-learning-for-tumor-detection-in-brain-MRI
A self-supervised learning framework for brain tumor classification using contrastive learning (SimCLR) with MRI scans.

## Overview
This project implements a self-supervised learning pipeline using SimCLR to learn meaningful representations from unlabeled MRI data, followed by linear evaluation for tumor classification. The model achieves **76.74% test accuracy** on the Brain Tumor MRI Dataset.

Key components:
- SimCLR implementation with ResNet-18 backbone
- Contrastive loss for representation learning
- Linear evaluation protocol
- PyTorch Lightning framework

## Dataset
Uses the [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) containing 4 classes:
- Glioma
- Meningioma
- No Tumor 
- Pituitary

Directory structure:
Training/
├── glioma/
├── meningioma/
├── notumor/
└── pituitary/
Testing/
└── (same structure)


## Features
- Dual-view data augmentation pipeline
- Feature extraction with ResNet-18
- Projection head for contrastive learning
- Linear classifier evaluation
- GPU acceleration support

## Installation
1. Clone repository:
```bash
git clone https://github.com/yourusername/brain-tumor-ssl.git
cd brain-tumor-ssl
