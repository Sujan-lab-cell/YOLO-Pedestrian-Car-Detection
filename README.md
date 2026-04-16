# 🌍 GeoSentinel AI: Smart Landslide Detection System

<p align="center">
<img src="https://img.shields.io/badge/Python-3.9-blue">
<img src="https://img.shields.io/badge/Framework-YOLOv8-green">
<img src="https://img.shields.io/badge/UI-Streamlit-orange">
<img src="https://img.shields.io/badge/Task-Landslide%20Detection-red">
</p>

---

## 📑 Table of Contents

* [Project Overview](#-project-overview)
* [Objectives](#-objectives)
* [Dataset Description](#-dataset-description)
* [Data Annotation](#-data-annotation)
* [Data Preprocessing and Augmentation](#-data-preprocessing--augmentation)
* [Model Architecture](#-model-architecture)
* [Training Configuration](#-training-configuration)
* [Training Performance](#-training-performance)
* [Model Performance Metrics](#-model-performance-metrics)
* [Confusion Matrix](#-confusion-matrix)
* [Precision–Recall Curve](#-precisionrecall-curve)
* [F1 Score Analysis](#-f1-score-analysis)
* [Detection Results](#-detection-results)
* [Real-World Image Evaluation](#-realworld-image-evaluation)
* [Failure Cases and Limitations](#-failure-cases-and-limitations)
* [Possible Improvements](#-possible-improvements)
* [Conclusion](#-conclusion)
* [Author](#-author)

---

# 📌 Project Overview

This project presents **GeoSentinel AI**, a deep learning-based system designed to detect **landslides** using the YOLOv8 segmentation model.

The system also includes:

* 📍 Map visualization (Folium)
* 📩 Alerts (SMS via Twilio, Email via SendGrid)
* 🎥 Video frame analysis
* 🔊 Voice alerts

Applications:

* Disaster management  
* Early warning systems  
* Environmental monitoring  

---

# 🎯 Objectives

* Build landslide dataset  
* Train YOLOv8 segmentation model  
* Detect landslides in real-time  
* Send alerts to authorities  
* Analyze performance  

---

# 📂 Dataset Description

Dataset includes:

* Satellite images  
* Drone footage  
* Terrain images  

### Dataset Characteristics

* Polygon mask annotations  
* Multi-environment coverage  
* Landslide & non-landslide data  

---

# 🏷️ Data Annotation

YOLO segmentation format using polygon masks for accurate region detection.

---

# 🔧 Data Preprocessing & Augmentation

### Preprocessing

* Image resizing (640×640)  
* Auto-orientation  

### Augmentation

* Flipping  
* Rotation  
* Brightness changes  
* Mosaic  

---

# 🧠 Model Architecture

Model: **YOLOv8 Segmentation (YOLOv8-Seg)**

Advantages:

* Fast  
* Accurate  
* Real-time capable  

---

# ⚙️ Training Configuration

| Parameter      | Value          |
| -------------- | -------------- |
| Model          | YOLOv8-Seg     |
| Image Size     | 640 × 640      |
| Epochs         | 100            |
| Batch Size     | 8              |
| IoU Threshold  | 0.45           |
| Confidence     | 0.50           |

---

# 📊 Training Performance

* Loss decreased steadily  
* mAP improved  
* Stable convergence  

### Training Graphs

<p align="center">
<img src="result/training_results.png" width="900">
</p>

---

# 📈 Model Performance Metrics

| Metric  | Value |
| ------- | ----- |
| Precision | High |
| Recall    | High |
| mAP       | Good |

---

# 📊 Confusion Matrix

<p align="center">
<img src="result/confusion_matrix.png" width="600">
</p>

Observations:

* Accurate detection  
* Minor errors in small regions  

---

# 📉 Precision-Recall Curve

<p align="center">
<img src="result/pr_curve.png" width="600">
</p>

Balanced precision and recall.

---

# 📊 F1 Score Analysis

<p align="center">
<img src="result/f1_curve.png" width="600">
</p>

---

# 🖼 Detection Results

<p align="center">
<img src="result/detection1.png" width="400">
<img src="result/detection2.png" width="400">
</p>

<p align="center">
<img src="result/detection3.png" width="400">
</p>

---

# 🌍 Real-World Image Evaluation

<p align="center">
<img src="result/realworld1.png" width="400">
<img src="result/realworld2.png" width="400">
</p>

Observations:

* Works in real-world conditions  
* Good generalization  

---

## ⚠️ Failure Cases and Limitations

### 1️⃣ False Negatives

<p align="center">
<img src="result/failure_false_negative.png" width="500">
</p>

### 2️⃣ False Positives

<p align="center">
<img src="result/failure_false_positive.png" width="500">
</p>

### 3️⃣ Occlusion

<p align="center">
<img src="result/failure_occlusion.png" width="500">
</p>

### 4️⃣ Small Objects

<p align="center">
<img src="result/failure_small_objects.png" width="500">
</p>

---

# 🚀 Possible Improvements

* ISRO satellite integration  
* Cloud deployment (AWS/GCP)  
* IoT rainfall sensors  
* GPS metadata extraction  
* Multi-user alerts  

---

# ✅ Conclusion

GeoSentinel demonstrates how AI can be used for real-time landslide detection.

✔ Accurate detection  
✔ Real-time alerts  
✔ Scalable system  

Helps reduce disaster impact and improve safety.

---

# 👨‍💻 Author

**Sujan KS**

Artificial Intelligence & Machine Learning  
Deep Learning & Computer Vision Enthusiast  

---
