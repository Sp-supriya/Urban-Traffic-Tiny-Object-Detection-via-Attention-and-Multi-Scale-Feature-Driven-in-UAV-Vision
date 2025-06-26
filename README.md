# RTS-NET: Real-Time Small Object Detection Network in UAV Vision 🚁🧠📦

A deep learning-based system designed to detect **tiny objects** in **UAV-captured urban traffic imagery** using an efficient and modular network architecture: **RTS-NET**.

---

## 📌 Project Overview

Unmanned Aerial Vehicles (UAVs) provide wide-area surveillance for traffic and urban monitoring. However, traditional object detection models fail to accurately detect **small or distant objects** (e.g., bikes, pedestrians, vehicles) due to resolution loss and background clutter.

**RTS-NET** addresses this problem by integrating:
- **MFFM**: Multi-Scale Feature Fusion Module  
- **CADM**: Channel Attention Deep Module  
- **RFEM**: Real-time Feature Extraction Module

Together, these components enable real-time, lightweight, and highly accurate detection of small objects.

---

## 🎯 Objectives

- Build a lightweight, high-speed detection model for real-time UAV vision.
- Improve small object detection using attention and feature fusion.
- Train and evaluate on a custom UAV-captured traffic dataset with 8 object classes.

---

## 🧠 Architecture

Input (UAV Image)
↓
Backbone CNN + RFEM
↓
MFFM (Multi-Scale Fusion)
↓
CADM (Channel/Spatial Attention)
↓
Detection Head (Class + Bounding Box)


- Model Input: 416×416 or 960×960 images  
- Output: Object labels with bounding boxes

---

## 🗂️ Dataset

- **Source**: UAV-captured urban traffic scenes
- **Classes**: Car, Bike, Truck, Pedestrian, Auto, Van, Bus, Traffic Sign
- **Annotations**: YOLO format
- **Split**: 70% Training | 20% Validation | 10% Testing

> *Alternative datasets like VisDrone and UAVDT can also be used for benchmarking.*

---

## 🔧 Tech Stack

- **Language**: Python  
- **Libraries**: TensorFlow/Keras, OpenCV, NumPy, Matplotlib  
- **Frontend**: OpenCV, Tkinter (or Web Interface)
- **Backend**: Django ORM (optional)
- **Database**: MySQL  
- **Deployment Tools**: TensorRT, ONNX (for edge deployment)

---

## 📊 Results

- ✅ **Accuracy**: 94% mAP on custom dataset
- 🕒 **Real-Time**: Optimized for live UAV feed (high FPS)
- 📉 **False Positives**: Minimal in complex traffic scenes
- 🚀 **Outperforms**: YOLOv5–YOLOv8, EfficientNet in tiny object tasks

---

## 📁 Project Structure

```bash
RTS-NET-UAV/
│
├── dataset/                   # Images & labels
├── models/                    # Model architecture files (MFFM, CADM, RFEM)
├── training/                  # Training scripts & logs
├── evaluation/                # Metrics, confusion matrix, mAP
├── detection/                 # Detection pipeline & utils
├── app/                       # Optional web or GUI interface
├── README.md                  # Project documentation
└── requirements.txt           # Python dependencies

🧪 Evaluation Metrics
mAP (mean Average Precision)

IoU (Intersection over Union)

FPS (Frames Per Second)

Precision / Recall / F1-Score

✅ Use Cases
Urban Traffic Monitoring

Disaster Rescue Detection

Agricultural Surveillance

Crowd Management in Smart Cities

🚀 Future Scope
Integrate multi-object tracking

Add video stream processing

Improve night/dark object visibility

Optimize for edge deployment on UAVs

🤝 Contributing
Pull requests are welcome! If you’d like to contribute, please fork the repo and submit a PR.

📜 License
This project is licensed under the MIT License.

📧 Contact
Author: Supriya

Email: [supriyasp1504@gmail.com]

LinkedIn: https://www.linkedin.com/in/supriya-sri-perambudhur-8a650725b/
