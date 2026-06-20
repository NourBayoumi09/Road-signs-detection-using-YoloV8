# Road Sign Detection using YOLOv8

## Overview

This project implements a road sign detection system using YOLOv8 for detecting and localizing traffic signs in images. The model was trained on a self-driving car dataset obtained from Roboflow and is designed as a computer vision component for autonomous driving and intelligent transportation systems.

## Dataset

The dataset was obtained from Roboflow Universe:

https://universe.roboflow.com/selfdriving-car-qtywx/self-driving-cars-lfjou

### Dataset Split

| Set | Images | Percentage |
|-------|--------:|-----------:|
| Training | 3,530 | 71% |
| Validation | 801 | 16% |
| Test | 638 | 13% |
| Total | 4,969 | 100% |

## Model

- Architecture: YOLOv8
- Task: Object Detection
- Framework: Ultralytics YOLOv8
- Input: Road images containing traffic signs
- Output: Bounding boxes and class labels

## Features

- Traffic sign detection and localization.
- Training and evaluation pipelines.
- Inference on unseen images.
- Visualization of predictions.
- Real-time object detection capability.

## Project Structure

```text
├── dataset/
├── runs/
├── Road_sign_detection_system_using_YOLO_8.ipynb
├── images/
├── requirements.txt
└── README.md
```

## Training

The model was trained on 3,530 images and validated on 801 images. Final evaluation was performed on a separate test set containing 638 images to assess generalization performance.

## Results

The model is capable of detecting and classifying traffic signs by predicting bounding boxes and corresponding classes. YOLOv8 provides a good trade-off between detection accuracy and inference speed, making it suitable for real-time applications.

## Applications

- Autonomous vehicles
- Advanced Driver Assistance Systems (ADAS)
- Traffic monitoring systems
- Smart transportation solutions
- Computer vision research

## Usage

Train the model:

```bash
yolo task=detect mode=train data=data.yaml model=yolov8n.pt epochs=100
```

Run inference:

```bash
yolo task=detect mode=predict model=best.pt source=path/to/image.jpg
```

## Technologies Used

- Python
- Ultralytics YOLOv8

## Dataset Citation

Self-Driving Cars Dataset  
Roboflow Universe  
https://universe.roboflow.com/selfdriving-car-qtywx/self-driving-cars-lfjou

## Acknowledgments

This project uses the Self-Driving Cars dataset provided by Roboflow Universe and the Ultralytics YOLOv8 framework for object detection.
