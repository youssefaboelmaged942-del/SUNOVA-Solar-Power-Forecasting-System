# SUNOVA: Solar Power Forecasting System

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Framework](https://img.shields.io/badge/FastAPI-Production--Ready-green.svg)
![Architecture](https://img.shields.io/badge/Model-Dual--Input%20LSTM-orange.svg)

An intelligent, end-to-end solar power generation forecasting solution leveraging deep learning sequence models and transfer learning across multiple photovoltaic (PV) plants.

---

## 📌 Project Overview
Forecasting solar power output is critical for grid stability, energy trading, and efficient integration of renewable energy sources. SUNOVA addresses the variability of solar generation by providing accurate short-term and medium-term predictions using data from **51 Photovoltaic (PV) plants**.

### Key Performance & Horizons
* **15-Minute Horizon:** Achieved **32.1% sMAPE** (significantly outperforming the 43.92% baseline).
* **24-Hour Horizon:** Reached a pooled **R² of 0.789** across 51 plants.

---

## 🏗 System Architecture & Workflow


```

[ Plant Metadata ] ───┐
├──► [ Dual-Input LSTM Architecture ] ──► [ FastAPI Backend ]
[ Weather & Power ] ──┘

```

1. **Dual-Input LSTM Network:** Simultaneously processes dynamic sequential data (weather parameters, solar geometry, lag, and rolling power metrics) and static plant metadata (nominal capacity, efficiency, geographic features).
2. **Transfer Learning Strategy:** Uses a fine-tuning approach across all 51 PV plants to improve generalization on unseen operational conditions.
3. **Model Serving:** Integrated into a high-performance, asynchronous **FastAPI** backend for low-latency real-time inference.

---

## 🛠 Tech Stack
* **Language & Core:** Python, NumPy, Pandas
* **Machine Learning & Deep Learning:** TensorFlow, Keras, Scikit-Learn
* **Model Architectures:** LSTM Networks, Random Forest (Baseline/Comparison)
* **API & Serving:** FastAPI, Uvicorn
* **Version Control:** Git, GitHub

---

## 📊 Key Features & Engineering
* **Feature Engineering:** Solar geometry parameters, temporal indicators, multi-step lag features, rolling statistics, and static site metadata.
* **Scalable Fine-Tuning:** Custom multi-plant transfer learning strategy for individual plant adaptation.
* **Production Serving:** REST API endpoints serving live predictions for short-term decision making.

---

## 👤 Author
**Youssef Abo El-Magd**  
*Junior AI & Data Analyst*  
* [LinkedIn](https://linkedin.com/in/youssef-abo-elmaged)
* [GitHub](https://github.com/youssefaboelmaged942-del)

```
