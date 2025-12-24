# 🫁 Project 1: Lung CT Scan Segmentation using SAM

## 📌 Overview
This project applies **Meta AI’s Segment Anything Model (SAM)** to **lung CT scan images** for medical image segmentation.  
The goal is to automatically segment lung regions from CT scans and visualize the results.


## 📂 Dataset
- **Dataset:** Chest CT Scan Images
- **Source:** Kaggle
- **Link:** https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

The dataset contains CT scan images categorized into different lung conditions.


## 🧠 Model
- **Model:** Segment Anything Model (SAM – ViT-B)
- **Checkpoint:** `sam_vit_b_01ec64.pth`
- **Framework:** PyTorch
- **Pretraining:** Large-scale image data


## ⚙️ Processing Pipeline
CT Scan Image
↓
Preprocessing
↓
SAM Image Encoder
↓
Prompt-based Segmentation
↓
Mask Generation
↓
Overlay Visualization


## 📊 Evaluation
- **Metric Used:** Intersection over Union (IoU)
- IoU is calculated where ground-truth masks are available.
- Results are primarily **qualitative**, focusing on segmentation accuracy and visual clarity.


## 🖼️ Sample Results
| Before | After |
|------|------|
| ![Before](results/lung/before.png) | ![After](results/lung/after.png) |



## 📁 Outputs
- Segmentation masks
- Overlay images (Before vs After)
- Saved results for visualization

