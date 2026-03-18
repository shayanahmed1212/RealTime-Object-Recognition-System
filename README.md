<div align="center">

<br/>

<!-- ═══════════════════ HERO BLOCK ═══════════════════ -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0f0f,50:1a1a2e,100:16213e&height=200&section=header&text=RealTime%20Object%20Recognition&fontSize=36&fontColor=00d4ff&fontAlignY=40&desc=Powered%20by%20YOLOv3%20%7C%20OpenCV%20%7C%20Python&descAlignY=62&descColor=a0a8c0" width="100%"/>

<br/>

<!-- ═══════════════════ BADGES ═══════════════════ -->
![Python](https://img.shields.io/badge/Python-3.8%2B-00d4ff?style=for-the-badge&logo=python&logoColor=white&labelColor=0f0f1a)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-00d4ff?style=for-the-badge&logo=opencv&logoColor=white&labelColor=0f0f1a)
![YOLOv3](https://img.shields.io/badge/YOLOv3-Darknet-00d4ff?style=for-the-badge&logo=darkreader&logoColor=white&labelColor=0f0f1a)
![License](https://img.shields.io/badge/License-MIT-00d4ff?style=for-the-badge&labelColor=0f0f1a)

<br/>

> **Real-time object detection** using YOLOv3 with Non-Maximum Suppression —  
> fast, accurate, and built for live camera feeds and HD video.

<br/>

</div>

---

<br/>

<!-- ═══════════════════ WHAT IT DOES ═══════════════════ -->
<table>
<tr>
<td width="50%" valign="top">

### 🎯 &nbsp;What It Does

This system captures live frames from any camera or video source, passes them through the **YOLOv3 neural network**, and overlays real-time bounding boxes with class labels and confidence scores — all in a single Python script.

- Detects **80+ object classes** from the COCO dataset
- Processes each frame with **Blob preprocessing** for consistent model input
- Eliminates duplicate detections using **NMS (Non-Maximum Suppression)**
- Runs efficiently on standard hardware without a dedicated GPU

</td>
<td width="50%" valign="top">

### ⚙️ &nbsp;How It Works

```
┌─────────────────────────────────────┐
│         Video Frame Input           │
│     (Webcam / Video File)           │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│    Blob Preprocessing (416×416)     │
│     Normalize + Resize Frame        │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│       YOLOv3 Forward Pass           │
│   3 Detection Scales (13/26/52)     │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│  NMS → Filter Overlapping Boxes     │
│  Draw Labels + Confidence Scores    │
└─────────────────────────────────────┘
```

</td>
</tr>
</table>

<br/>

---

## 🚀 &nbsp;Getting Started

<br/>

### &nbsp;Step 1 — Download Model Weights

> The YOLOv3 weights file is **~236 MB** and cannot be stored in this repository.

<div align="center">

[![Download Weights](https://img.shields.io/badge/⬇%20Download-yolov3.weights%20(236MB)-00d4ff?style=for-the-badge&labelColor=1a1a2e)](https://drive.google.com/file/d/1g2qaORkUhd4hmGN67CNOb6tLKHOrazQl/view?usp=sharing)

</div>

<br/>

### &nbsp;Step 2 — Set Up Project Directory

Place all four files in **the same folder**:

```
📁 your-project/
├── 🐍  main.py            ← Python execution script
├── ⚖️  yolov3.weights     ← Downloaded from the link above
├── 🔧  yolov3.cfg         ← Model architecture config
└── 🏷️  coco.names         ← 80 COCO class labels
```

> ⚠️ **Important:** The script resolves model paths relative to its own directory.  
> All YOLO files must be in the **same folder** as `main.py`.

<br/>

### &nbsp;Step 3 — Install Dependencies

```bash
pip install opencv-python numpy
```

<br/>

### &nbsp;Step 4 — Run the System

```bash
python main.py
```

<br/>

---

## ✨ &nbsp;Key Features

<br/>

<table>
<tr>

<td align="center" width="33%">

**🎥 Real-Time Processing**

Highly optimized pipeline for live camera feeds and high-definition video files with minimal latency per frame.

</td>

<td align="center" width="33%">

**🧠 YOLOv3 Architecture**

Multi-scale detection at **13×13**, **26×26**, and **52×52** grids. Detects small, medium, and large objects simultaneously.

</td>

<td align="center" width="33%">

**🎯 NMS Integration**

Non-Maximum Suppression removes redundant overlapping boxes, keeping only the highest-confidence detection per object.

</td>

</tr>
</table>

<br/>

---

## 📋 &nbsp;Prerequisites

| Requirement | Version |
|---|---|
| Python | 3.8 or higher |
| opencv-python | 4.x |
| numpy | Any recent |
| OS | Windows / macOS / Linux |

<br/>

---

## 📁 &nbsp;Required YOLO Files

| File | Source | Purpose |
|---|---|---|
| `yolov3.weights` | [Google Drive ↗](https://drive.google.com/file/d/1g2qaORkUhd4hmGN67CNOb6tLKHOrazQl/view?usp=sharing) | Pre-trained model weights (~236 MB) |
| `yolov3.cfg` | Included in repo | Network architecture definition |
| `coco.names` | Included in repo | 80 object class labels |

<br/>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0f0f0f&height=100&section=footer" width="100%"/>

<sub>Built with OpenCV + YOLOv3 · COCO Dataset · Non-Maximum Suppression</sub>

</div>
