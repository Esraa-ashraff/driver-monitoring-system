# 🚗 Driver Monitoring System (DMS) 

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.8+-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/Model-YOLOv8-red.svg" alt="YOLOv8">
  <img src="https://img.shields.io/badge/Library-OpenCV-green.svg" alt="OpenCV">
  <img src="https://img.shields.io/badge/Tools-MediaPipe-teal.svg" alt="MediaPipe">
</p>

An advanced, real-time AI-powered system designed to enhance road safety by monitoring driver attentiveness. This project was awarded **1st Place** at the Benha University Student Conference (2025).

---

## 📌 Project Overview
The system utilizes Computer Vision and Deep Learning to analyze driver behavior in real-time. It is specifically engineered to handle complex real-world variables that often challenge standard monitoring models.

### Core Detection Capabilities:
- **Drowsiness Detection:** Real-time monitoring of eye closure duration with immediate alerts.
- **Distraction Tracking:** Precise 3D head pose estimation (Looking Left, Right, Up, or Down).
- **Environmental Robustness:** High-accuracy performance even when the driver is wearing **Masks** or **Glasses**.

---

## 🎯 Features
* **YOLOv8 Multi-Model Pipeline:** Integration of 3 specialized YOLOv8 models for Face Mask, Glasses, and Eye Status detection.
* **3D Head Pose Estimation:** Leverages MediaPipe Face Mesh and PnP (Perspective-n-Point) algorithm for accurate orientation tracking.
* **Intelligent Alert System:** Instant audio warnings via `pygame` triggered by time-based thresholds to minimize false positives.
* **High Performance:** Optimized for real-time processing with high FPS (Frames Per Second) stability.

---

## 🛠️ Technical Stack
* **Programming:** Python
* **AI/ML:** YOLOv8 (Ultralytics), MediaPipe
* **Computer Vision:** OpenCV, NumPy
* **Audio Processing:** Pygame (Mixer)
* **Mathematics:** 3D Projection Matrices & Euclidean Distance

---

## 📂 Project Structure
```text
├── Code/
│   └── main.py              # Core system logic and state machine
├── Models/
│   ├── best.pt              # Glasses detection model weights
│   ├── Mask.pt              # Face mask detection model weights
│   └── closed.pt            # Eye status detection for masked faces
├── Sounds/
│   ├── left.wav             # Audio alert files
│   ├── Right.wav
│   ├── down.wav
│   └── Warningg.mp3
└── requirements.txt         # Project dependencies
```
---

## 🚀 Getting Started

### 1. Installation
Clone the repository and install the necessary dependencies:

```bash
git clone (https://github.com/Esraa-ashraff/driver-monitoring-system.git)
cd driver-monitoring-system
pip install -r requirements.txt
```
---

### 2. Running the Project
Ensure your camera is connected and the model, sound files are located in the same folder of the code, then execute:

```bash
python Code/main.py
```
---

---

## 📊 Results & Demo
The system classifies driver states into 5 distinct categories for maximum safety coverage: 

* **Face Detected:** Normal driving state (Forward-facing).
* **Face with Glasses:** Successful tracking while wearing eyewear.
* **Face with Mask:** Accurate eye tracking optimized for masked faces.
* **Face with Mask and Glasses:** Handling complex overlapping conditions.
* **No Face Detected:** Immediate warning triggered when no face is visible to the camera.

### 🎬 Project Demo
[Click here to watch the full project demo on Google Drive](https://drive.google.com/file/d/1kayAskRXusCPOulKT4XsajhBqONFXQkW/view?usp=drive_link)

---

## 🏆 Achievements
* **Award:** 1st Place Winner - Benha University Student Conference (2025).
* **Academic Grade:** A+ (Excellent with Honors) for Graduation Project.

---

## 📬 Contact
**Esraa Ashraf** 📧 **Email:** [esraashraf09@gmail.com](mailto:esraashraf09@gmail.com)  
🔗 **LinkedIn:** [Connect with me](https://www.linkedin.com/in/esraa-ashraf-ba5573300/)
