# 🎙️ Namaste Tarang — Edge Keyword Spotting

<p align="center">

### ⚡ Low-Latency & Lightweight Voice Activation for Edge Devices

**Custom Wake Word:** `Namaste Tarang`

</p>

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-D00000?style=for-the-badge&logo=keras&logoColor=white)
![TinyML](https://img.shields.io/badge/TinyML-Edge%20AI-6A1B9A?style=for-the-badge)
![ESP32](https://img.shields.io/badge/Target-ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)

</p>

---

## 🌟 Overview

**Namaste Tarang** is a lightweight **Keyword Spotting (KWS)** system designed to detect the custom wake phrase:

> 🎤 **"Namaste Tarang"**

The project focuses on bringing voice activation closer to the **edge**, where a compact machine-learning model can continuously listen for a wake phrase without requiring continuous cloud-based inference.

The model uses **MFCC-based audio features** and a compact **Convolutional Neural Network (CNN)** designed with resource-constrained deployment in mind.

---

## 🎯 Objective

The system is being developed for **low-latency voice activation on edge devices**, with deployment targeted toward hardware such as the **ESP32**.

The core pipeline is:

```text
🎙️ Microphone
      │
      ▼
🔊 Audio Capture
      │
      ▼
🎛️ Preprocessing
      │
      ▼
📊 MFCC Feature Extraction
      │
      ▼
🧠 Lightweight CNN
      │
      ▼
⚡ Wake / Not-Wake
      │
      ▼
🚀 Edge Device Activation
