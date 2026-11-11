# Industrial Fire & Smoke Detection System

A real-time industrial fire and smoke detection system built using Python, OpenCV, PyTorch, and YOLOv8. The system combines computer vision techniques to identify potential fire and smoke hazards, monitor surrounding objects, and display real-time safety information.

---

## Developer

**Pragati Sarang**

GitHub: https://github.com/pragatisarang36-design

---

## Project Overview

This project focuses on real-time monitoring and detection of fire and smoke in industrial environments using computer vision.

It uses HSV-based colour segmentation for fire detection, motion analysis and frame differencing for smoke detection, and YOLOv8 for identifying people and vehicles in the surrounding scene.

---

## Key Features

- **Fire Detection:** HSV colour segmentation to identify fire regions using red, orange, and yellow colour ranges.
- **Smoke Detection:** Motion analysis, background subtraction, frame differencing, and grey-tone colour masking.
- **Object Detection:** YOLOv8-based detection of people, cars, buses, and trucks.
- **Risk Classification:** Categorizes detected hazards into CLEAR, CAUTION, WARNING, and CRITICAL levels.
- **Real-Time Monitoring:** Displays detection results and safety information through a visual monitoring interface.
- **Visual Alerts:** Highlighted hazard regions, detection bounding boxes, and animated warning banners.
- **Performance Monitoring:** Displays FPS, processing latency, and detection confidence.
- **GPU Support:** Supports GPU acceleration with CPU fallback.

---

## Tech Stack

- Python
- OpenCV
- YOLOv8 (Ultralytics)
- PyTorch
- Torchvision
- NumPy
- Pillow

---

## Project Structure

```text
Industrial-Fire-and-Smoke-Detection-System/
│
├── app.py
├── yolov8n.pt
└── README.md
```

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/pragatisarang36-design/Industrial-Fire-and-Smoke-Detection-System.git
```

### 2. Navigate to the Project Directory

```bash
cd Industrial-Fire-and-Smoke-Detection-System
```

### 3. Run the Application

```bash
python app.py
```

The application automatically checks for and installs its required Python packages if they are missing.

---

## Usage

The system supports multiple video sources:

**Webcam:**

```bash
python app.py
```

**Video File:**

```bash
python app.py video.mp4
```

**RTSP Stream:**

```bash
python app.py rtsp://your-stream-url
```

### Available Controls

| Key | Function |
|---|---|
| Q | Quit the application |
| P | Pause / Resume |
| S | Capture screenshot |

The processed video is saved as `output_detected.mp4` by default.

To specify a different output filename:

```bash
python app.py video.mp4 --output result.mp4
```

To disable YOLO scene detection:

```bash
python app.py --no-yolo
```

---

## Project Goal

To develop a computer vision-based safety monitoring system capable of identifying potential fire and smoke hazards in real time and providing visual alerts to support industrial safety monitoring.

---

## Note

This project is intended for educational and research purposes. It should not be considered a replacement for certified industrial fire detection and safety systems.
