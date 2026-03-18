# RealTime-Object-Recognition-System

A real-time object detection system built with Python, OpenCV, and YOLOv3. Features optimized frame processing and Non-Maximum Suppression (NMS) for clean, accurate detections.

## 🚀 Getting Started

Due to the large file size, the YOLOv3 pre-trained weights could not be included directly in this repository. You must download them manually to run the system.

### 📦 Prerequisites & Model Weights

1.  **Download the Weights:** <a href="https://drive.google.com/file/d/1g2qaORkUhd4hmGN67CNOb6tLKHOrazQl/view?usp=sharing" target="_blank">Download yolov3.weights from Google Drive</a>

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
🛠️ Installation & Usage
Install the required libraries:

Bash
pip install opencv-python numpy
Run the detection script:

Bash
python main.py
⚙️ Key Features
Real-time Processing: Highly optimized for live camera feeds or high-definition video files.

YOLOv3 Architecture: Utilizes the state-of-the-art YOLOv3 model for high-speed, high-accuracy object detection.

NMS Integration: Uses Non-Maximum Suppression to eliminate overlapping bounding boxes, ensuring only the most accurate detections are displayed.


---

### Why this works:
* **One-Click Install:** I put the `pip` command in a code block so users can copy-paste it instantly.
* **Feature Highlights:** I expanded on the YOLOv3 and Real-time points to make the project look more professional to anyone visiting your GitHub.

Would you like me to add a **"How it Works"** section that briefly explains what YOLO
