# AI-Powered Predictive Maintenance System 🛠️🤖

A Machine Learning-based Predictive Maintenance pipeline that analyzes real-time sensor data from industrial machinery to predict equipment failures before they happen, helping minimize downtime and optimize maintenance scheduling.

---

## 📌 Project Overview
This project provides an end-to-end Machine Learning solution designed to predict machine failures, estimate remaining useful life, and analyze repair costs using industrial sensor telemetry.

It consists of an **Interactive Web Application (`app.py`)** powered by **trained Machine Learning Pipelines (`.pkl` models)** that perform real-time predictions:
1. **24-Hour Failure Prediction:** Foresees whether a machine will fail within the next 24 hours.
2. **Failure Type Classification:** Identifies the root cause or specific type of failure.
3. **Remaining Useful Life (RUL) Estimation:** Predicts the remaining operational hours before breakdown.
4. **Estimated Repair Cost:** Calculates potential maintenance costs to assist in budget planning.

---

## ✨ Key Features
* **Failure Prediction (Binary Classification):** Detects potential breakdown risks 24 hours in advance.
* **Failure Mode Analysis (Multi-class Classification):** Identifies specific failure types (e.g., heat dissipation, power failure, tool wear, overstrain).
* **RUL & Cost Forecasting (Regression Models):** Estimates remaining running hours and expected repair expenses.
* **Interactive Web Dashboard (`app.py`):** Simple interface for entering machine parameters and getting instant predictions.
* **Pre-packaged Scikit-Learn Pipelines:** Serialized models handling feature scaling, preprocessing, and inference.

---

## 📁 Repository Structure


predictive_maintenance/
│
├── models/
│   ├── failure_24h_pipeline.pkl
│   ├── failure_type_pipeline.pkl
│   ├── repair_cost_pipeline.pkl
│   └── rul_pipeline.pkl
│
├── notebooks/
│   ├── failure_within_24.ipynb
│   ├── failure_type.ipynb
│   ├── estimated_repair_cost.ipynb
│   └── rul_hours.ipynb
│
├── predictive_maintenance_v3.csv
├── app.py
├── requirements.txt
├── Industrial_Predictive_Maintenance_Presentation.pptx
├── .gitattributes
└── README.md


## 🚀 Getting Started
1. Prerequisites & Installation
Ensure you have Python 3.8+ installed. Clone the repository and install the dependencies:

## Bash
# Clone the repository
git clone [https://github.com/mohamedgameel21/AI-Powered-Predictive-Maintenance-System-for-Industrial-Equipment.git](https://github.com/mohamedgameel21/AI-Powered-Predictive-Maintenance-System-for-Industrial-Equipment.git)
cd predictive_maintenance

# Install required libraries
pip install -r requirements.txt
2. Run the Web Application
Launch the web interface using Streamlit:

Bash
streamlit run app.py
## 🛠️ Tech Stack
Language: Python

Data Analysis & Preprocessing: Pandas, NumPy

Machine Learning & Modeling: Scikit-Learn, PyTorch

Model Tracking: Git LFS

Web Interface: Streamlit
