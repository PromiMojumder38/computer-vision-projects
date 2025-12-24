# 🧠📹 Computer Vision Projects (Medical Imaging & Traffic Analysis)

This repository contains two end-to-end **Computer Vision projects** demonstrating practical skills in **image segmentation**, **video-based object detection**, and **model deployment workflows** using modern deep learning models.

The projects were developed using **PyTorch**, **foundation vision models**, and **Google Colab**, with a strong focus on **documentation, reproducibility, and real-world data**.

---

## 📁 Projects Overview

| Project | Domain | Model | Task |
|------|------|------|------|
| Lung CT Scan Segmentation | Medical Imaging | SAM (Segment Anything) | Image Segmentation |
| Traffic Video Analysis | Video Analytics | YOLOv8 | Object Detection |

---

# 🫁 Project 1: Lung CT Scan Segmentation using SAM

## 📌 Overview
This project applies **Meta AI’s Segment Anything Model (SAM)** to **lung CT scan images** for medical image segmentation.  
The goal is to automatically segment lung regions from CT scans and visualize the results.

---

## 📂 Dataset
- **Dataset:** Chest CT Scan Images
- **Source:** Kaggle
- **Link:** https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

The dataset contains CT scan images categorized into different lung conditions.

---

## 🧠 Model
- **Model:** Segment Anything Model (SAM – ViT-B)
- **Checkpoint:** `sam_vit_b_01ec64.pth`
- **Framework:** PyTorch
- **Pretraining:** Large-scale image data

---

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


---

## 📊 Evaluation
- **Metric Used:** Intersection over Union (IoU)
- IoU is calculated where ground-truth masks are available.
- Results are primarily **qualitative**, focusing on segmentation accuracy and visual clarity.

---

## 🖼️ Sample Results
| Before | After |
|------|------|
| ![Before](results/lung/before.png) | ![After](results/lung/after.png) |

---

## 📁 Outputs
- Segmentation masks
- Overlay images (Before vs After)
- Saved results for visualization

---

# 🚗 Project 2: Traffic Video Object Detection using YOLOv8

## 📌 Overview
This project demonstrates **real-world traffic video analysis** using **YOLOv8** for object detection.  
A publicly available **YouTube traffic surveillance video** is used as input, and the model processes the video frame-by-frame to generate an annotated output video.

---

## 🎥 Input Video
- **Source:** Public YouTube traffic camera
- **YouTube Link:**  
https://www.youtube.com/watch?v=7LrWGGJFEJo

> The video was downloaded programmatically using `yt-dlp`.

---

## 🧠 Model
- **Model:** YOLOv8 Nano (`yolov8n.pt`)
- **Framework:** Ultralytics YOLO
- **Pretraining:** COCO dataset
- **Reason for choice:** Fast inference suitable for video processing

---

## ⚙️ Processing Pipeline
YouTube Video
↓
Video Download (yt-dlp)
↓
Frame-by-frame Processing
↓
YOLOv8 Object Detection
↓
Annotated Output Video


---

## 📊 Detected Classes
- Cars
- Trucks
- Motorcycles
- Persons

(Classes depend on COCO dataset labels.)

---

## 📁 Output
The output video contains:
- Bounding boxes
- Class labels
- Frame-by-frame detections

📥 **Annotated Output Video:**  
[Download traffic_annotated.mp4](/Traffic%20Video%20Annotation/traffic_annotated.mp4)


## 🖼️ Sample Output Frame
![Traffic Detection](results/traffic/sample_frame.png)

---

## 🚀 How to Run
1. Open the notebook in **Google Colab**
2. Download dataset / video
3. Run the notebook cells sequentially
4. Outputs will be saved locally


## 🛠️ Technologies Used
- Python
- PyTorch
- Ultralytics YOLOv8
- Segment Anything (SAM)
- OpenCV
- NumPy
- Matplotlib
- Google Colab


## 📌 Notes
- All datasets and videos used are **publicly available**
- No private or sensitive data is used
- Projects are intended for **educational and research purposes**



## ✅ Why This Repository Matters
This repository demonstrates:
- Practical application of **foundation vision models**
- Experience with **medical image segmentation**
- Video-based **real-time object detection**
- Strong emphasis on **documentation and reproducibility**
- Readiness for **research assistant and CV-focused roles**

