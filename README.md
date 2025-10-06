# Pneumonia Detection System using Deep Learning and VOC Sensor Integration

This repository contains the design and implementation of a hybrid pneumonia detection system that combines **deep learning–based image classification** with **real-time breath analysis using VOC sensors**. The project demonstrates an interdisciplinary integration of **AI, IoT, and biomedical engineering** for early, non-invasive pneumonia detection.

---

## Overview

Pneumonia is a severe respiratory infection that requires rapid diagnosis for effective treatment. Traditional methods like X-rays and blood tests are expensive, time-consuming, and often expose patients to radiation.  
This project introduces a **dual-diagnostic approach**:
1. **AI-based detection** from chest X-rays using Convolutional Neural Networks (CNNs).  
2. **Sensor-based detection** using exhaled breath analysis to identify elevated levels of biomarkers such as **CO₂**, **NO**, and **volatile organic compounds (VOCs)**.

---

## Objectives

- Develop and evaluate deep learning models (VGG16, MobileNetV2, DenseNet121, InceptionV3) for pneumonia detection using chest X-rays.
- Integrate a low-cost VOC sensing device for non-invasive detection via breath analysis.
- Create a hybrid diagnostic pipeline combining AI and sensor-based inference.
- Ensure compatibility with embedded hardware (ESP32) for real-time monitoring and wireless data transfer.
- Promote accessibility, sustainability, and affordability in medical diagnostics.

---

## System Architecture

1. **Data Input**  
   - Dataset: Pediatric chest X-ray dataset (5,863 images) from Mendeley Data.  
   - Categories: Normal (1,341) and Pneumonia (4,522).  

2. **Deep Learning Pipeline**  
   - Frameworks: TensorFlow, Keras, OpenCV.  
   - Models trained with Adam optimizer and categorical cross-entropy loss.  
   - Regularization using dropout, batch normalization, and learning-rate scheduling.  
   - **MobileNetV2 achieved the best accuracy of 90.9%**, followed by VGG16 (90.2%).

3. **Hardware Integration**  
   - Microcontroller: ESP32  
   - Sensors:  
     - MiCS 5524 – VOC detection  
     - MiCS 2714 – NO₂ detection  
     - SCD40 D R2 – CO₂ detection  
   - Power: Dual 3.3V lithium-ion batteries (7.4V total, regulated to 5V via buck converter).  
   - Communication: Wi-Fi-enabled data transfer for remote diagnostics.

4. **PCB Design**  
   - Designed using KiCad for compact, low-power operation.  
   - Includes filters, voltage dividers, and I²C communication for sensor interfacing.

---

## Tools and Parameters

| Category | Tools/Parameters |
|-----------|------------------|
| **Software** | Python, TensorFlow, Keras, OpenCV, Matplotlib, Seaborn |
| **Hardware** | ESP32 microcontroller, VOC, NO₂, and CO₂ sensors |
| **Simulation** | HFSS / KiCad (hardware), Google Colab (software) |
| **Training** | Batch size: 32, Epochs: 50, Optimizer: Adam, Loss: Categorical Cross-Entropy |

---

## Results

| Model | Accuracy (%) | Suitability |
|--------|---------------|-------------|
| MobileNetV2 | 90.9 | Best for embedded deployment |
| VGG16 | 90.2 | Strong baseline model |
| DenseNet121 | 88.0 | Efficient, but heavier |
| InceptionV3 | 86.2 | High accuracy, more resource-intensive |

The integrated VOC detection device successfully identifies spikes in exhaled compounds corresponding to respiratory distress. Combined with CNN-based image inference, the hybrid system provides reliable, real-time detection without invasive procedures.

---

## Social and Environmental Impact

- **Healthcare Accessibility:** Enables portable, low-cost diagnosis in remote or underserved areas.  
- **Environmental Benefit:** Reduces reliance on radiological equipment, minimizing radiation exposure.  
- **Sustainability:** Low-power sensors and embedded systems contribute to green medical technology.  
- **Educational Value:** Encourages interdisciplinary research in AI, biomedical engineering, and IoT.

---

## Alignment with UN Sustainable Development Goals

- **SDG 3:** Good Health and Well-being  
- **SDG 9:** Industry, Innovation, and Infrastructure  
- **SDG 10:** Reduced Inequalities  
- **SDG 4:** Quality Education (Indirect)

---

## Contributors

- **Rupam Mal** – Deep Learning and Software Development  
- **Harsh Kumar** – Cross-domain Documentation and Integration  
- **Debtonu Bose** – Hardware Design, Circuit Development, and Sensor Integration  
- **Guide:** Dr. Prachi Sharma  

---

## References

Key supporting literature from peer-reviewed journals and IEEE/Elsevier sources on FPGA-based biomedical imaging, VOC sensing, and deep learning optimization for medical diagnostics.  
(Full list available in the project documentation folder.)

---

## Repository Structure

