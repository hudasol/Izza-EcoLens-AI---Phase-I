# 🌍 EcoLens AI: Phase 1 (Edge-Computing & ESG Compliance)

**EcoLens AI** is a decentralized, edge-computing framework designed for verifiable source-segregation and real-time carbon accounting. This repository focuses on the implementation of the **Waste Intelligence Monitor**, integrating RTSP IP camera streams with a blockchain-inspired audit log for ESG (Environmental, Social and Governance) reporting.

---

## 📂 Repository Structure

```text
EcoLens-AI-Phase2/
├── 📂 .github/               # CI/CD workflows for ESG compliance auditing
├── 📂 core/                  # [Proprietary] Edge-computing & RTSP stream logic
│   ├── 🐍 camera_stream.py   # RTSP IP Camera integration (OpenCV/BGR-to-RGB)
│   └── 🐍 processor.py       # Log processing and SHA-256 hash generation
├── 📂 dashboard/             # [Proprietary] Streamlit Waste Intelligence UI
│   └── 🐍 app.py             # Main UI for real-time monitoring & KPIs
├── 📂 data/                  # Audit logs and metadata
│   ├── 📄 ecolens_audit_log.csv # Blockchain-verified event log
│   └── 📄 classes.txt        # Classification labels (PET, Alum, etc.)
├── 📂 models/                # [Proprietary] TFLite quantized weights
│   └── 📄 model.tflite       # Edge-optimized inference model
├── 📄 .gitignore             # Prevents sensitive .csv and .env leaks
├── 📄 LICENSE                # Academic & Commercial usage terms
├── 📄 README.md              # Documentation & Implementation Guide
└── 📄 requirements.txt       # Dependencies (OpenCV, Streamlit, Pandas)


## 🧠 Core System Architecture

### 1. Edge-AI Perception
The core utilizes a **TFLite quantized model** optimized for low-latency inference on edge devices (e.g., Raspberry Pi). The engine performs real-time classification into six distinct waste streams:
* **Recyclables:** PET Plastic, Aluminum, Paper.
* **Non-Recyclables:** General Waste, Organic, and Specialty Handling.

### 2. Immutable Audit Trail
To align with **UAE Federal Decree-Law No. 11 (2024)**, every classification event is logged with cryptographic integrity:
* **Temporal Tracking:** Precise Timestamp & Category logging. 
* **Environmental Impact:** Real-time calculation of CO₂ prevention metrics.
* **Cryptographic Hashing:** Every entry is linked via **SHA-256 anchoring**, creating a tamper-proof ledger of waste diversion for sustainability audits.

### 3. Waste Intelligence Monitor
A **Streamlit-powered dashboard** provides real-time visualization of sustainability KPIs. It translates raw telemetry into actionable business insights, such as the estimated monetary value (**AED**) of diverted waste and equivalent energy savings.

---

## ⚖️ Compliance & Sustainability
EcoLens AI is engineered to support organizational **GHG (Greenhouse Gas) reporting**. By quantifying diverted waste into CO₂-equivalent savings, the platform enables enterprises to meet international sustainability standards (**GRI/SASB**) and local UAE environmental regulations.
