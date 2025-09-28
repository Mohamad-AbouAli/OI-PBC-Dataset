# Comprehensive Benchmarking of YOLOv11 for Peripheral Blood Cell Detection

[![arXiv](https://img.shields.io/badge/arXiv-Preprint-b31b1b)](https://arxiv.org/abs/XXXX.XXXXX)
[![License](https://img.shields.io/badge/License-ACM-blue)](LICENSE)
[![YOLOv11](https://img.shields.io/badge/YOLO-v11-red)](https://github.com/ultralytics/ultralytics)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://python.org)
[![Dataset](https://img.shields.io/badge/Dataset-16,891%20images-orange)](https://github.com/Mohamad-AbouAli/OI-PBC-Dataset)

## 📖 Overview

This repository contains the official implementation for **"Comprehensive Benchmarking of YOLOv11 Architectitectures for Scalable and Granular Peripheral Blood Cell Detection"** (submitted to ArXiv). Our research provides a rigorous evaluation of YOLOv11 models for automated detection and classification of 12 peripheral blood cell types using a large-scale annotated dataset.

**Key Findings:**
- 🎯 **YOLOv11-Medium** achieves optimal balance with **93.4% mAP@0.5**
- 📊 **8:1:1 data split** consistently outperforms traditional 7:2:1 split
- ⚡ **Diminishing returns** observed beyond Medium variant
- 🏥 **Clinical-ready** model selection for hematology applications

## 🚀 Quick Start

### Google Colab Notebooks
We provide ready-to-use Colab notebooks for easy experimentation:

- [`Training_YOLOv11_Blood_Cells.ipynb`](Colab_Notebooks/Training_YOLOv11_Blood_Cells.ipynb) - Train models from scratch
- [`Inference_Demo.ipynb`](Colab_Notebooks/Inference_Demo.ipynb) - Run inference on new images
- [`Performance_Evaluation.ipynb`](Colab_Notebooks/Performance_Evaluation.ipynb) - Evaluate model performance

### Quick Inference
```python
from ultralytics import YOLO

# Load our pre-trained model
model = YOLO('models/yolov11m_blood_cells.pt')

# Run detection
results = model('path/to/blood_smear.jpg', conf=0.5)
results[0].show()
