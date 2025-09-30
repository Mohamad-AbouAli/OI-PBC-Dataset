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

## Citation

If you find our work or dataset useful, please consider citing our preprint:

```bibtex
@article{abouali2025comprehensive,
  title={Comprehensive Benchmarking of YOLOv11 Architectures for Scalable and Granular Peripheral Blood Cell Detection},
  author={Abou Ali, Mohamad and Abdulfattah, Mariam and Al Hussein, Baraah and Dornaika, Fadi and Cherry, Ali and Hajj-Hassan, Mohamad and Hamawy, Lara},
  journal={arXiv preprint arXiv:2509.24595},
  year={2025}}
}

**Quick Access:**
- 🔗 [Read Paper](https://arxiv.org/abs/2509.24595)
