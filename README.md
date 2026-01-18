# UIDAI-PROJECT

An AI-powered risk intelligence system designed to analyze Aadhaar biometric and demographic update patterns and highlight regions that may require closer scrutiny.

---

## 🔍 Motivation

Aadhaar update systems process large volumes of biometric and demographic changes daily.  
Manual monitoring cannot reliably detect subtle, coordinated, or time-based irregularities.

This project introduces an **intelligent, data-driven framework** to surface potential risk patterns early and present them in an interpretable manner.

---

## 🧠 System Overview

The system transforms raw update records into **explainable risk intelligence** by combining:

- Behavioral anomaly detection
- Temporal pattern learning
- Spatial risk aggregation

The final output is a **risk-aware dashboard** designed for decision-makers.

---

## 🤖 Models & Techniques Used

### 1️⃣ Behavioral Intelligence
**Isolation Forest**
- Detects abnormal update behavior
- Flags unexpected biometric-to-demographic ratios
- Works without labeled fraud data

**Why used:**  
Effective for unsupervised anomaly detection in large-scale systems.

---

### 2️⃣ Temporal Intelligence
**LSTM (Long Short-Term Memory)**
- Learns update trends over time per pincode
- Distinguishes short-term spikes from sustained anomalies

**Why used:**  
Captures long-term dependencies that simple rolling statistics miss.

---

### 3️⃣ Spatial Intelligence
- Aggregation across state, district, and pincode levels
- Highlights geographic clustering of elevated risk

**Why used:**  
Risk often emerges as spatial concentration rather than isolated points.

---

## 📊 Risk Scoring Logic

Final Risk Score is derived from a weighted combination of:

- Behavioral anomaly score
- Temporal deviation score
- Spatial intensity score

### Interpretation:
| Risk Score | Meaning |
|-----------|--------|
| < 0.30 | Normal |
| 0.30 – 0.47 | Elevated |
| > 0.47 | High Risk |

These thresholds are chosen to reflect **realistic operational risk**, not theoretical extremes.

---

## 📈 Dashboard Highlights

- State & district level filtering
- Risk heatmaps for intuitive spatial insight
- Time-series anomaly visualization
- Clear explanation of what each score represents

Built using **Streamlit** for clarity and ease of presentation.

---

## 🗂 Repository Structure

How to Run
1️⃣ Clone repository
git clone https://github.com/<your-username>/UIDAI-PROJECT.git
cd UIDAI-PROJECT

2️⃣ Create environment
conda create -n uidai python=3.9
conda activate uidai
conda install -c conda-forge pandas numpy scikit-learn tensorflow matplotlib seaborn streamlit

3️⃣ Run notebook

Execute the Jupyter notebook to generate processed outputs

4️⃣ Launch dashboard
streamlit run app.py
