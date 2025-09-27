# T1_G45_Tensor_Tacticians
# Sentiment Recognition via Facial Cues and Neural Signals

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.8%2B-purple.svg)](https://python.org)  
[![XGBoost](https://img.shields.io/badge/XGBoost-1.6%2B-red.svg)](https://xgboost.readthedocs.io/)  
[![Performance](https://img.shields.io/badge/Performance-93%25-success.svg)](#outcomes)  
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

</div>

> **Cutting-edge dual-modal sentiment detection framework integrating neural wave analysis with facial micro-expression recognition achieving 93% classification performance.**

## 🎯 System Overview

This framework addresses the complex challenge of sentiment classification through the fusion of dual modalities:
- **Neural signals**: Processing brainwave activity and electrical patterns
- **Facial micro-expressions**: Evaluating facial features through Affectiva analysis

**Primary Achievement**: 93% classification performance utilizing sophisticated feature extraction and XGBoost methodology.

## 🏗️ Framework Design

```mermaid
graph TD
    A[Neural Signals] --> D[Feature Extraction]
    B[Facial Micro-expressions<br/>Affectiva] --> D
    C[TIVA Dataset] --> D
    
    D --> E[Variance Filtering]
    E --> F[Correlation<br/>Elimination]
    F --> G[XGBoost Feature<br/>Ranking Top 45]
    
    G --> H[Class Distribution<br/>Balancing]
    H --> I[SMOTE Generation]
    H --> J[Weight Adjustment]
    
    I --> K[XGBoost Model]
    J --> K
    
    K --> L[Sentiment Detection<br/>93% Performance]
    
    %% Modified theme styling
    style A fill:#4c1d95,stroke:#8b5cf6,stroke-width:2px,color:#ffffff
    style B fill:#991b1b,stroke:#ef4444,stroke-width:2px,color:#ffffff
    style C fill:#064e3b,stroke:#34d399,stroke-width:2px,color:#ffffff
    style D fill:#701a75,stroke:#d946ef,stroke-width:2px,color:#ffffff
    style E fill:#1e293b,stroke:#64748b,stroke-width:2px,color:#ffffff
    style F fill:#1e293b,stroke:#64748b,stroke-width:2px,color:#ffffff
    style G fill:#1e293b,stroke:#64748b,stroke-width:2px,color:#ffffff
    style H fill:#991b1b,stroke:#fca5a5,stroke-width:2px,color:#ffffff
    style I fill:#1e293b,stroke:#64748b,stroke-width:2px,color:#ffffff
    style J fill:#1e293b,stroke:#64748b,stroke-width:2px,color:#ffffff
    style K fill:#155e63,stroke:#22d3ee,stroke-width:2px,color:#ffffff
    style L fill:#047857,stroke:#059669,stroke-width:3px,color:#ffffff


flowchart LR
    A[Raw Neural Data] --> B[Temporal Window<br/>Segmentation<br/>1-5s]
    C[Facial Attributes<br/>TIVA.csv] --> B
    
    B --> D[Feature Synchronization<br/>& Fusion]
    D --> E[Data Processing &<br/>Preparation]
    E --> F[Feature Extraction<br/>Framework]
    
    F --> G[Model Development<br/>& Assessment]
    
    %% Modified theme with green accent
    style A fill:#059669,stroke:#34d399,stroke-width:2px,color:#ffffff
    style B fill:#1e293b,stroke:#10b981,stroke-width:2px,color:#ffffff
    style C fill:#059669,stroke:#34d399,stroke-width:2px,color:#ffffff
    style D fill:#1e293b,stroke:#10b981,stroke-width:2px,color:#ffffff
    style E fill:#1e293b,stroke:#10b981,stroke-width:2px,color:#ffffff
    style F fill:#1e293b,stroke:#10b981,stroke-width:2px,color:#ffffff
    style G fill:#047857,stroke:#6ee7b7,stroke-width:3px,color:#ffffff


sentiment-recognition/
├── data/
│   ├── EEG.csv              # Neural brainwave attributes
│   └── TIVA.csv             # Facial expression dataset
├── notebooks/
│   ├── 01_preprocessing.ipynb        # Data preparation & processing
│   ├── 02_feature_engineering.ipynb  # Feature ranking & selection
│   └── 03_modeling_baseline.ipynb    # XGBoost framework
└── README.md 

