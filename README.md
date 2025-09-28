# Comprehensive Benchmarking of YOLOv11 for Peripheral Blood Cell Detection

[![arXiv](https://img.shields.io/badge/arXiv-Preprint-b31b1b)](https://arxiv.org/abs/XXXX.XXXXX)
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

## 📁 Repository Structure
├── Colab_Notebooks/ # Google Colab notebooks
│ ├── Training_YOLOv11_Blood_Cells.ipynb
│ ├── Inference_Demo.ipynb
│ └── Performance_Evaluation.ipynb
├── Dataset/
│ ├── 721_split/ # 70:20:10 split
│ ├── 811_split/ # 80:10:10 split
│ └── annotations/ # Multiple formats (VOC, YOLO, CSV)
├── Models/ # Pre-trained weights
│ ├── yolov11n_blood_cells.pt
│ ├── yolov11s_blood_cells.pt
│ ├── yolov11m_blood_cells.pt
│ ├── yolov11l_blood_cells.pt
│ └── yolov11x_blood_cells.pt
├── Results/ # Evaluation results
│ ├── confusion_matrices/
│ ├── performance_curves/
│ └── quantitative_results/
├── LICENSE
└── README.md

## 🛠️ Installation & Usage
**Prerequisites**

# Install required packages
pip install ultralytics torch torchvision opencv-python pandas numpy matplotlib



## 📈 Results & Recommendations

### Key Findings
- **YOLOv11-Medium achieves the best accuracy-efficiency trade-off**
- **8:1:1 split provides better performance across all models**
- **Smaller models benefit more from additional training data**
- **Diminishing returns beyond Medium variant**

### Clinical Recommendation
For real-world hematology applications, we recommend:

- **Model**: YOLOv11-Medium
- **Data Split**: 8:1:1
- **Performance**: 93.4% mAP@0.5 with practical computational requirements

## 🎯 Performance Highlights

- **High Precision**: 92.6% precision for rare cell detection
- **Excellent Recall**: 93.9% recall minimizing false negatives
- **Robust Performance**: Consistent across all 12 cell classes
- **Clinical Relevance**: Suitable for integration into diagnostic workflows
