Overview

This project implements a road sign detection system using YOLOv8. The model is trained to detect and classify traffic signs from images, which is an essential component of autonomous driving and intelligent transportation systems.

The dataset consists of images collected for self-driving car applications and contains multiple traffic sign categories. YOLOv8 was used because of its balance between speed and detection accuracy, making it suitable for real-time applications.

Dataset

The dataset was obtained from Roboflow Universe:

Source:
https://universe.roboflow.com/selfdriving-car-qtywx/self-driving-cars-lfjou

Dataset Split
Set	Images	Percentage
Training	3,530	71%
Validation	801	16%
Test	638	13%
Total	4,969	100%
Model
Architecture: YOLOv8
Task: Object Detection
Framework: Ultralytics YOLOv8
Input: Road images containing traffic signs
Output: Bounding boxes and class labels for detected signs
Features
Traffic sign detection and localization.
Training, validation, and testing pipelines.
Support for inference on new images.
Visualization of predictions with bounding boxes.
Suitable for autonomous driving and computer vision applications.
Project Structure
├── dataset/
├── runs/
├── models/
├── notebooks/
│   └── Road_sign_detection_system_using_YOLO_8.ipynb
├── images/
├── results/
├── requirements.txt
└── README.md
Training

The model was trained using the Ultralytics implementation of YOLOv8 on the training dataset containing 3,530 images. Performance was monitored using a validation set of 801 images, and final evaluation was performed on a separate test set of 638 images.

Applications
Autonomous vehicles
Advanced Driver Assistance Systems (ADAS)
Traffic monitoring systems
Smart transportation solutions
Computer vision research

Requirements:

Python 3.x
Ultralytics YOLOv8

Dataset: 

Self-Driving Cars Dataset
Roboflow Universe
https://universe.roboflow.com/selfdriving-car-qtywx/self-driving-cars-lfjou
Acknowledgments

This project uses the Self-Driving Cars dataset provided by Roboflow Universe and the Ultralytics YOLOv8 framework for object detection.
