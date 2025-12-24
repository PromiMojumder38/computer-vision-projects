
# 🚗 Project 2: Traffic Video Object Detection using YOLOv8

## 📌 Overview
This project demonstrates **real-world traffic video analysis** using **YOLOv8** for object detection.  
A publicly available **YouTube traffic surveillance video** is used as input, and the model processes the video frame-by-frame to generate an annotated output video.

## 🎥 Input Video
- **Source:** Public YouTube traffic camera
- **YouTube Link:**  
https://www.youtube.com/watch?v=CftLBPI1Ga4

> The video was downloaded programmatically using `yt-dlp`.

## 🧠 Model
- **Model:** YOLOv8 Nano (`yolov8n.pt`)
- **Framework:** Ultralytics YOLO
- **Pretraining:** COCO dataset
- **Reason for choice:** Fast inference suitable for video processing

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


## 📊 Detected Classes
- Cars
- Trucks
- Motorcycles
- Persons

(Classes depend on COCO dataset labels.)

## 📁 Output
The output video contains:
- Bounding boxes
- Class labels
- Frame-by-frame detections

📥 **Annotated Output Video:**  
https://github.com/PromiMojumder38/computer-vision-projects/blob/main/Traffic%20Video%20Annotation/traffic_annotated.gif


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



