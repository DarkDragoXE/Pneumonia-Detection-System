<div align="center">

# Pneumonia Detection System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org)
[![ESP32](https://img.shields.io/badge/Hardware-ESP32-red.svg)](https://www.espressif.com/en/products/socs/esp32)
[![Accuracy](https://img.shields.io/badge/Accuracy-90.9%25-brightgreen.svg)](/)
[![Capstone](https://img.shields.io/badge/VIT-Capstone%20Project-purple.svg)](/)

### Deep Learning + IoT-Based Hybrid Diagnostic System

**A non-invasive, AI-powered pneumonia detection system combining chest X-ray analysis with real-time breath biomarker monitoring**

[Overview](#overview) | [Features](#key-features) | [Results](#results) | [Hardware](#hardware-design) | [Team](#team) | [Author](#author)

</div>

---

## About

This is the **B.Tech Capstone Project** developed at VIT Vellore from December 2024 to May 2025. The project demonstrates a novel hybrid approach combining deep learning for chest X-ray analysis with IoT-based breath biomarker monitoring for non-invasive pneumonia detection.

| | |
|---|---|
| **Institution** | VIT Vellore |
| **Duration** | December 2024 - May 2025 |
| **Team Size** | 3 |
| **Role** | Team Lead |
| **Tools** | KiCad, VSCode, TensorFlow |

### Key Achievements

- Developed **ESP32-based portable device** integrating VOC, NO2, and CO2 sensors
- Designed **power circuitry** using dual 3.3V lithium-ion batteries with buck converter
- Deployed **MobileNetV2 CNN model** (90.9% accuracy) on embedded hardware
- Created affordable alternative to traditional radiological methods
- Non-invasive pneumonia detection through breath biomarker analysis

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
| **Power** | Dual 3.3V Li-ion + Buck Converter | Stable sensor operation |

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
| **Debtonu Bose** | Team Lead, Hardware Engineer |
| **Rupam Mal** | ML Engineer |
| **Harsh Kumar** | Integration and Documentation |

**Guide**: Dr. Prachi Sharma | **Capstone Project 2024-2025**

---

## Author

**Debtonu Bose**
B.Tech Electronics and Communication Engineering
Vellore Institute of Technology (2021-2025)

[![GitHub](https://img.shields.io/badge/GitHub-DarkDragoXE-black?logo=github)](https://github.com/DarkDragoXE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-debtonu--bose-blue?logo=linkedin)](https://linkedin.com/in/debtonu-bose)

---

## Future Work

- [ ] Deploy on ESP32 with TensorFlow Lite
- [ ] Develop mobile app
- [ ] Clinical validation
- [ ] Bacterial vs viral classification

---

<div align="center">

**VIT Vellore | Capstone Project | 2024-2025**

</div>
