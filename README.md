# Final Term — Medical Image Segmentation: Dermatitis

This project focuses on segmenting inflamed skin regions (dermatitis) in medical images using deep learning techniques.

- **Kaggle Notebook**: [View here](https://www.kaggle.com/code/zzz3103/finalterm-medical-segmentation)  
- **Public Dataset Accuracy**: **0.9142** (evaluated on 30% of the dataset)  
- **Private Dataset Accuracy**: **0.9401** (evaluated on 100% of the dataset)  

---

## Overview

The goal of this project is to accurately segment dermatitis regions from skin images using a U‑Net-based convolutional neural network. The workflow includes:

1. Preprocessing and augmentation of images  
2. Building and training a segmentation model  
3. Evaluation using both public and private leaderboards on Kaggle

---

## Dataset

- The dataset contains medical skin images along with ground-truth segmentation masks that label inflamed (dermatitis) areas.
- The data is split into a **public** portion (30%) for intermediate evaluation and a **private** portion (100%) for final scoring.

---

## Model

- **Architecture**: U‑Net with a ResNeSt269e pretrained encoder  
- **Loss Function**: Dice Loss + Binary Cross-Entropy Loss  
- **Optimizer**: Adam  
- **Evaluation Metric**: Dice Coefficient

---

## Results

| Metric               | Public Score | Private Score |
|----------------------|--------------|---------------|
| **Dice Coefficient** | 0.9142       | 0.9401        |
