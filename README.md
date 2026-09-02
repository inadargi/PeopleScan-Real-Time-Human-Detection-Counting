# 🚶 PeopleScan: Real-Time Human Detection & Counting 🔍

A deep learning-based project for detecting and counting humans in videos, images, or live camera feeds. 🎥📸🤖

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-DeepLearning-green?logo=opencv&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📑 Table of Contents
- [🧠 Overview](#-overview)
- [✨ Features](#-features)
- [⚙️ Requirements](#️-requirements)
- [🚀 Installation](#-installation)
- [▶️ Usage](#️-usage)
- [🏷️ Command Line Arguments](#️-command-line-arguments)
- [💡 Examples](#-examples)
- [📤 Output](#-output)

## 🧠 Overview

This project uses a deep learning-based human detection model to identify and count the number of people present in a given input — whether it's a 🎬 video file, a 🖼️ static image, or a 📹 live camera feed. Detected humans are highlighted with bounding boxes, and the total count is displayed/reported in real time. ⚡

## ✨ Features

- 🎬 Detect and count humans in **video files**
- 🖼️ Detect and count humans in **static images**
- 📹 Real-time detection using a **live camera feed**
- 💾 Option to **save the output** (annotated video/image) to a file

## ⚙️ Requirements

- 🐍 Python 3.x
- 👁️ OpenCV
- 🔢 NumPy
- 🛠️ imutils
- 🧩 A pre-trained human detection model (e.g., HOG + SVM or a deep learning-based detector such as MobileNet-SSD)

## 🚀 Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd human-detection-counting
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## ▶️ Usage

Run `main.py` with the appropriate flag depending on your input source.

### 1️⃣ Video File as Input
```bash
python main.py -v 'Path_to_video'
```

### 2️⃣ Image File as Input
```bash
python main.py -i 'Path_to_image'
```

### 3️⃣ Camera Feed as Input
```bash
python main.py -c True
```

### 4️⃣ Save the Output
```bash
python main.py -c True -o 'file_name'
```

## 🏷️ Command Line Arguments

| Flag | Description |
|---|---|
| 🎬 `-v` | Path to the input video file |
| 🖼️ `-i` | Path to the input image file |
| 📹 `-c` | Set to `True` to use the live camera feed |
| 💾 `-o` | Output file name to save the detection results |

## 💡 Examples

```bash
# 🎬 Detect and count humans in a video
python main.py -v 'videos/street.mp4'

# 🖼️ Detect and count humans in an image
python main.py -i 'images/crowd.jpg'

# 📹 Use webcam for real-time detection
python main.py -c True

# 💾 Use webcam and save the annotated output
python main.py -c True -o 'output.avi'
```

## 📤 Output

- 🟩 Each detected human is marked with a bounding box in the output frame/image.
- 🔢 The total human count is displayed on the output feed/image.
- 💾 If the `-o` flag is used, the annotated output is saved to the specified file name.

---

⭐ *If you find this project useful, consider giving it a star!*
🐛 *Feel free to raise an issue or submit a pull request for improvements or bug fixes.*
