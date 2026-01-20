<div align="center">

# Pneumonia Detection System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org)
[![ESP32](https://img.shields.io/badge/Hardware-ESP32-red.svg)](https://www.espressif.com/en/products/socs/esp32)
[![Accuracy](https://img.shields.io/badge/Accuracy-90.9%25-brightgreen.svg)](/)
[![Capstone](https://img.shields.io/badge/VIT-Capstone%20Project-purple.svg)](/)

### Deep Learning + IoT-Based Hybrid Diagnostic System

**A non-invasive, AI-powered pneumonia detection system combining chest X-ray analysis with real-time breath biomarker monitoring**

[Overview](#overview) | [Features](#key-features) | [Results](#results) | [Hardware](#hardware-design) | [Team](#team)

</div>

---

## Overview

Pneumonia is a severe respiratory infection affecting millions worldwide. This capstone project introduces a **dual-diagnostic approach**:

| Approach | Method | Technology |
|----------|--------|------------|
| **AI Detection** | Chest X-ray Classification | CNN (MobileNetV2, VGG16) |
| **Breath Analysis** | Exhaled Biomarker Detection | VOC/NO2/CO2 Sensors |

---

## Key Features

- **High Accuracy**: MobileNetV2 achieves **90.9% accuracy**
- **Non-Invasive**: Breath analysis eliminates radiation exposure
- **Portable**: ESP32-based point-of-care diagnostics
- **Low-Cost**: Affordable for developing regions
- **Real-Time**: Wireless data transfer

---

## System Architecture

<div align="center">
<img src="images/system_architecture.jpeg" alt="System Architecture" width="800"/>
</div>

---

## Deep Learning Models

| Model | Accuracy | Best For |
|-------|----------|----------|
| **MobileNetV2** | **90.9%** | Embedded deployment |
| VGG16 | 90.2% | Baseline/Server |
| DenseNet121 | 88.0% | Balanced |
| InceptionV3 | 86.2% | High accuracy needs |

### Model Comparison

<div align="center">
<img src="images/model_comparison.png" alt="Model Comparison" width="700"/>
</div>

---

## Results

### Training Performance

<div align="center">
<table>
<tr>
<td><img src="images/training_results_1.png" width="400"/></td>
<td><img src="images/training_results_2.png" width="400"/></td>
</tr>
</table>
</div>

### Confusion Matrices

<div align="center">
<table>
<tr>
<td><img src="images/confusion_matrix_1.png" width="400"/></td>
<td><img src="images/confusion_matrix_2.png" width="400"/></td>
</tr>
</table>
</div>

---

## Hardware Design

| Component | Model | Function |
|-----------|-------|----------|
| **MCU** | ESP32 | Processing + Wi-Fi |
| **VOC Sensor** | MiCS 5524 | VOC detection |
| **NO2 Sensor** | MiCS 2714 | NO2 measurement |
| **CO2 Sensor** | SCD40 | CO2 monitoring |

### Circuit Schematics

<div align="center">
<table>
<tr>
<td><img src="hardware/schematics/circuit_schematic.jpeg" width="400"/></td>
<td><img src="hardware/schematics/power_distribution.jpeg" width="400"/></td>
</tr>
</table>
</div>

---

## Documentation

**[Final Presentation (PDF)](docs/presentation/Final%20Review%20PPT.pdf)**

---

## Team

**VIT Vellore** - School of Electronics Engineering (SENSE)

| Name | Role |
|------|------|
| **Rupam Mal** | ML Engineer |
| **Harsh Kumar** | Integration and Documentation |
| **Debtonu Bose** | Hardware Engineer |

**Guide**: Dr. Prachi Sharma | **Capstone Project 2024-2025**

---

## Future Work

- [ ] Deploy on ESP32 with TensorFlow Lite
- [ ] Develop mobile app
- [ ] Clinical validation

---

<div align="center">

**VIT Vellore | 2024-2025**

</div>
