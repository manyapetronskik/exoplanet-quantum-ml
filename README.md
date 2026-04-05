# 🌌 Quantum-Enhanced Exoplanet Detection

## 🚀 Overview

This project explores exoplanet detection using real astronomical light curve data from the NASA.
The goal is to identify whether a star hosts an exoplanet based on brightness variations over time.

The project compares three approaches:

* Classical Machine Learning
* Deep Learning (LSTM)
* Quantum Machine Learning (Variational Quantum Classifier)

---

## 📊 Problem Statement

Exoplanet detection is a **rare-event classification problem**:

* Majority class → No planet
* Minority class → Planet

This leads to **extreme class imbalance**, making accurate detection challenging.

---

## 🧠 Approach

### 🔹 1. Classical Machine Learning

* Feature Engineering:

  * Mean, Standard Deviation
  * Transit Depth
  * Skewness, Kurtosis
* Models:

  * Random Forest
* Observation:

  * High accuracy but failed to detect planets

---

### 🔹 2. Deep Learning (LSTM)

* Used raw time-series light curve data

* Captured temporal dependencies

* Applied class weighting

* Observation:

  * Improved detection but unstable due to limited data

---

### ⚛️ 3. Quantum Machine Learning

* Implemented using Qiskit

* Model: Variational Quantum Classifier (VQC)

* Reduced features to match qubit constraints

* Applied **SMOTE** for class balancing

* Observation:

  * Achieved balanced precision and recall
  * Demonstrated potential of quantum models in scientific data analysis

---

## 📈 Results Summary

| Model                 | Performance                     |
| --------------------- | ------------------------------- |
| Classical ML          | Failed to detect minority class |
| LSTM                  | High recall but unstable        |
| Quantum (VQC + SMOTE) | Balanced precision & recall     |

---

## 🛠️ Tech Stack

* Python
* Scikit-learn
* TensorFlow / Keras
* Qiskit
* NumPy, Pandas, Matplotlib

---

## ⚠️ Key Challenges

* Extreme class imbalance
* Limited positive samples
* Noisy astronomical data
* Quantum model limitations (qubits, depth)

---

## 💡 Key Insights

* Accuracy is misleading for imbalanced datasets
* Recall is critical for rare-event detection
* Data quality impacts all models more than architecture
* Quantum models require careful data preparation

---

## 🌠 Future Work

* Use larger datasets (TESS / Kepler full dataset)
* Improve feature engineering
* Hybrid quantum-classical architectures
* Experiment with deeper quantum circuits

---

## 📂 Project Structure

```
├── README.md
├── classic_ml_lstm.ipynb
├── quantum_vqc_model.ipynb
├── requirements.txt
```

---

## 👩‍💻 Author

Medha Shekar K
AI/ML Engineer | Aspiring Quantum Computing Researcher ✨
