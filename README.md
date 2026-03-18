# RealTime-Object-Recognition-System

A real-time object detection system built with Python, OpenCV, and YOLOv3. Features optimized frame processing and Non-Maximum Suppression (NMS) for clean, accurate detections.

## 🚀 Getting Started

Due to the large file size, the YOLOv3 pre-trained weights could not be included directly in this repository. You must download them manually to run the system.

### 📦 Prerequisites & Model Weights

1.  **Download the Weights:** [Download yolov3.weights from Google Drive](https://drive.google.com/file/d/1g2qaORkUhd4hmGN67CNOb6tLKHOrazQl/view?usp=sharing)

2.  **Required Files:**
    Ensure you have the following three core YOLO files:
    * `yolov3.weights` (Downloaded from the link above)
    * `yolov3.cfg` (The configuration file)
    * `coco.names` (The list of object class names)

### 📂 Directory Structure

**Important:** For the script to locate the model correctly, all model-related files must be placed in the **same directory** as your main Python script. Your project folder should look like this:

```text
.
├── main.py                 # Your Python execution script
├── yolov3.weights          # The file downloaded from Google Drive
├── yolov3.cfg              # Configuration file
└── coco.names              # Class labels file
