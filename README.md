# 👁️ Person Detection System using YOLOv8

![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-red?style=flat-square)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

Real-time person detection system built with 
YOLOv8 pretrained on COCO dataset. Detects and 
locates persons in images, videos, and live webcam 
with bounding boxes and confidence scores.

---

## 🎯 Features

- ✅ Detect persons in any image
- ✅ Process video files with annotated output
- ✅ Real-time webcam detection (auto-starts)
- ✅ Confidence threshold analysis
- ✅ Person count overlay on every frame
- ✅ Confidence score distribution chart
- ✅ Works on CPU — no GPU required

---

## 📊 Model Performance

| Metric | Score |
|---|---|
| Model | YOLOv8n (pretrained COCO) |
| mAP@0.5 | 0.525 |
| Person mAP | ~0.65 |
| Speed | ~6ms/image (CPU) |
| Parameters | 3.2M |

---

## 🛠️ Tech Stack

- Python 3.9+
- Ultralytics YOLOv8
- OpenCV
- Matplotlib
- Pillow
- NumPy

---

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/engineerzainabbas/person-detection-yolov8.git
cd person-detection-yolov8
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run detection on an image
```python
from ultralytics import YOLO
import cv2

model = YOLO('yolov8n.pt')
results = model('your_image.jpg', conf=0.25, classes=[0])
results[0].show()
```

### 4. Run webcam detection
```python
# Open the notebook and run Step 9
# Webcam starts automatically
```

---

## 📂 Project Structure
```
person-detection-yolov8/
│
├── person_detection_yolov8_v2.ipynb  ← Main notebook
├── requirements.txt                   ← Dependencies
├── README.md                          ← This file
├── test_images/                       ← Sample images
│   ├── bus.jpg
│   └── zidane.jpg
└── results/                           ← Output images
    ├── detection_bus.png
    ├── detection_zidane.png
    ├── confidence_threshold_analysis.png
    ├── model_metrics_comparison.png
    └── detection_statistics.png
```

---

## 🔮 How to Use

### Detect in any image
```python
predict_persons('your_image.jpg')
predict_persons('your_image.jpg', conf=0.4)
```

### Detect in video
```python
detect_in_video('your_video.mp4')
```

### Live webcam (auto-starts)
```python
webcam_detection()
```

---

## 📸 Sample Results

| Input | Persons Detected | Confidence |
|---|---|---|
| bus.jpg | 4 persons | 0.85 avg |
| zidane.jpg | 2 persons | 0.91 avg |

---

## 🏭 Real-World Applications

- 🏪 **Retail** — Customer counting & foot traffic
- 🏭 **Factories** — Worker safety monitoring
- 🔒 **Security** — Intruder detection systems
- 🏥 **Hospitals** — Patient movement tracking
- 🚗 **Parking** — Occupancy detection
- 🌾 **Events** — Crowd density analysis

---

## ⚠️ Disclaimer

This project is for educational purposes only.

---

## 👤 Author

**Zain Abbas**
- 🎓 Computer Engineering
- 💼 AI & Machine Learning Engineer
- 🔗 [LinkedIn](https://www.linkedin.com/in/engineerzainabbas/)
- 📧 engineerzainabbas@gmail.com

---

## 📄 License

This project is licensed under the MIT License.
```
