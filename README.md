# AI-Powered Predictive Maintenance System 🛠️🤖

A Machine Learning-based Predictive Maintenance pipeline that analyzes real-time sensor data from industrial machinery to predict equipment failures before they happen, helping minimize downtime and optimize maintenance scheduling.

---

## 📌 Project Overview
This project provides an end-to-end Machine Learning solution designed to predict machine failures and categorize the specific type of failure using industrial sensor telemetry.

It consists of a **Web Application (`app.py`)** powered by **trained Machine Learning Pipelines (`.pkl` models)** that perform real-time predictions:
1. **24-Hour Failure Prediction:** Foresees whether a machine will fail within the next 24 hours.
2. **Failure Type Classification:** Classifies the root cause or specific type of failure to assist maintenance engineers in taking swift, targeted actions.

---

## ✨ Key Features
* **Failure Prediction (Binary Classification):** Detects potential breakdown risks 24 hours in advance.
* **Failure Mode Analysis (Multi-class Classification):** Identifies specific failure types (e.g., heat dissipation, power failure, tool wear, overstrain).
* **Interactive Web Dashboard (`app.py`):** Simple interface for entering machine parameters and getting instant predictions.
* **Pre-packaged Scikit-Learn Pipelines:** Serialized models (`failure_24h_pipeline.pkl`, `failure_type_pipeline.pkl`) handling feature scaling, preprocessing, and inference.

---

## 📁 Repository Structure
---
Predictive-Maintenance/

│
├── models/
│   ├── rul_pipeline.pkl
│   ├── repair_cost_pipeline.pkl
│   ├── failure_type_pipeline.pkl
│   └── failure_24h_pipeline.pkl
│
├── notebooks/
│   ├── rul_hours.ipynb
│   ├── failure_within_24.ipynb
│   ├── failure_type.ipynb
│   └── estimated_repair_cost.ipynb
│
├── screenshots/
│   ├── app_1.png
│   └── app_2.png
│
├── app.py
├── requirements.txt
├── predictive_maintenance_v3.csv
├── Industrial_Predictive_Maintenance_Presentation.pptx
├── .gitattributes
└── README.md
## 🚀 Getting Started

### 1. Prerequisites
Ensure you have Python 3.8+ installed along with the required libraries:
```bash
pip install numpy pandas scikit-learn streamlit
