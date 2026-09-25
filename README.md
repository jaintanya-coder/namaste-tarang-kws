# 🎙️ Namaste Tarang — Edge Keyword Spotting

<p align="center">
  <img src="https://img.shields.io/badge/TinyML-Edge%20AI-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/TensorFlow-Keras-orange?style=for-the-badge&logo=tensorflow">
  <img src="https://img.shields.io/badge/Target-ESP32-green?style=for-the-badge&logo=espressif">
</p>

> **A lightweight keyword spotting system for detecting the custom wake phrase _"Namaste Tarang"_ on resource-constrained edge devices.**

## ⚡ Highlights

- 🎙️ Custom **"Namaste Tarang"** wake-word detection
- 🧠 Lightweight **CNN with depthwise-separable convolutions**
- 🎵 **40 MFCC** features extracted from 16 kHz audio
- ⚡ **INT8 TensorFlow Lite** quantization for edge deployment
- 🔌 Designed for **ESP32**
- 📊 Includes confusion matrix, classification report & threshold analysis
- 🚀 Includes **TFLite inference benchmarking**

## 🔄 Pipeline

```text
Audio → Preprocessing → MFCC → Lightweight CNN → Wake / Not Wake
                                      ↓
                              INT8 TFLite → ESP32

🧠 Model
| Parameter | Value |
|---|---|
| Sample Rate | 16 kHz |
| Audio Length | 3.7 sec |
| Features | 40 MFCC |
| Architecture | Lightweight CNN |
| Output | Wake / Not Wake |
| Quantization | INT8 |
| Target | ESP32 |

🛠️ Tech Stack
Python · TensorFlow · Keras · Librosa · Scikit-learn · TensorFlow Lite · ESP32

📁 Repository
namaste-tarang-kws/
├── 📓 namaste-tarang-kws.ipynb
└── 📄 README.md
The training dataset is kept private and is not included in this repository.

🎯 Project Context
Developed for ISRO Problem Statement PS ID 26172 —
"Low Latency and Efficient Voice Activator for Edge Devices."
The notebook contains the complete workflow from audio preprocessing → model training → evaluation → INT8 conversion → edge inference benchmarking.

<p align="center">
  🎙️ <b>Speech → AI → Edge</b> ⚡
</p>
```
