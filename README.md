# 🎙️ Namaste Tarang — Edge Keyword Spotting

<p align="center">
  <img src="https://img.shields.io/badge/TinyML-Edge%20AI-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/TensorFlow-Keras-orange?style=for-the-badge&logo=tensorflow">
  <img src="https://img.shields.io/badge/ESP32-Edge%20Deployment-green?style=for-the-badge&logo=espressif">
</p>

<p align="center">
  <b>Low-Latency Keyword Spotting for Resource-Constrained Edge Devices</b>
</p>

> 🎤 Detecting the custom wake phrase **"Namaste Tarang"** using a lightweight neural network designed for edge deployment.

---

## ⚡ Project Highlights

- 🎙️ Custom **"Namaste Tarang"** wake-word detection
- 🧠 Lightweight **CNN with depthwise-separable convolutions**
- 🎵 **40 MFCC** features from 16 kHz audio
- ⚡ **INT8 TensorFlow Lite** quantization
- 🔌 Target deployment: **ESP32**
- 📊 Confusion matrix, classification report & threshold analysis
- 🚀 TFLite inference benchmarking

---

## 🔄 Pipeline

```text
🎙️ Audio
   ↓
Preprocessing
   ↓
40 MFCC Features
   ↓
Lightweight CNN
   ↓
┌───────────────┬───────────────┐
│   NOT WAKE    │     WAKE      │
│      ❌       │      🟢       │
└───────────────┴───────────────┘
                    ↓
             INT8 TFLite
                    ↓
                 ESP32
```

---

## 🧠 Model Configuration

| Parameter | Value |
|---|---|
| Sample Rate | **16 kHz** |
| Audio Duration | **3.7 sec** |
| Features | **40 MFCCs** |
| Model | Lightweight CNN |
| Classes | `wake` / `not_wake` |
| Quantization | **INT8** |
| Target Device | **ESP32** |

---

## 🛠️ Tech Stack

**Python · TensorFlow · Keras · Librosa · NumPy · Scikit-learn · TensorFlow Lite · ESP32**

---

## 📊 Evaluation

The notebook includes:

- Confusion Matrix
- Classification Report
- Precision / Recall / F1-score
- Wake-word probability threshold analysis
- INT8 model size & quantization details
- TFLite inference latency benchmarking

---

## 📁 Repository Structure

```text
namaste-tarang-kws/
│
├── 📓 namaste-tarang-kws.ipynb
└── 📄 README.md
```

🔒 **Dataset:** The training dataset contains private audio recordings and is therefore **not included in this repository**.

---

## 🎯 Project Context

Developed for **ISRO Problem Statement PS ID 26172**:

> **"Low Latency and Efficient Voice Activator for Edge Devices"**

The project explores an end-to-end edge AI pipeline:

**Audio → Feature Extraction → CNN → Quantization → Edge Inference**

---

