# ⭐ GRB Light Curve Reconstruction – NAOJ Winter Research Internship (2024–25)

**Author:** Debanik Debnath  
**Institute:** National Astronomical Observatory of Japan (NAOJ)  
**Mentor:** Prof. Maria Giovanna Dainotti (SOKENDAI / NAOJ)  
**Duration:** December 2024 – February 2025 (Remote)

---

## 🔭 Overview

This repository documents my research contributions during my Winter Internship at the **National Astronomical Observatory of Japan (NAOJ)**. The project focused on reconstructing **Gamma-Ray Burst (GRB) X-ray afterglow light curves** using:

* Classical statistical models
* Machine learning regression
* Deep learning architectures (LSTM, Bi-LSTM, GRU, CNN-LSTM, Transformers)
* Hybrid and probabilistic pipelines

The objective was to improve reconstruction fidelity and extract key astrophysical parameters such as:

* Plateau end time (log Tₐ)
* Flux at plateau (log Fₐ)
* Temporal decay slopes
* Light-curve smoothness and discontinuities

This work contributes to a broader cosmological effort to evaluate GRBs as potential **standardizable candles** for studying the expansion of the high-redshift universe.

---

## 📚 Primary Scientific References

### **1. Gamma-Ray Burst Light Curve Reconstruction (arXiv)**

[https://arxiv.org/abs/2412.20091](https://arxiv.org/abs/2412.20091)
*A multi-model framework for reconstructing GRB light curves using machine and deep-learning approaches.*
This includes models closely related to my LSTM / Bi-LSTM pipeline designs.

### **2. Dainotti et al. (2023) – ApJS 267, 42**

[https://ui.adsabs.harvard.edu/abs/2023ApJS..267...42D/abstract](https://ui.adsabs.harvard.edu/abs/2023ApJS..267...42D/abstract)
*A foundational study on GRB X-ray afterglows, plateau correlations, and cosmological implications.*
This paper heavily influenced the modeling direction of my internship.

### **3. Dainotti et al. – GRB Standardization Work**

[https://ui.adsabs.harvard.edu/abs/2023ApJS..267...42D/abstract](https://ui.adsabs.harvard.edu/abs/2023ApJS..267...42D/abstract)
*Further methodological inspiration for GRB classification, data preprocessing, and statistical handling.*

---

## 🎯 My Key Contributions

### ✔ Processed and analyzed **200+ GRB light curves**

* Trimming, cleaning, normalization, time-binning, and multi-epoch comparison.

### ✔ Built multiple deep-learning architectures

* LSTM (baseline + optimized)
* **Bi-LSTM** (best-performing, bidirectional temporal context)
* GRU
* 1D-CNN
* CNN-LSTM hybrids
* Autoencoders & Denoising AEs
* Transformer-based experiments

### ✔ Classical & Probabilistic Techniques

* Gaussian Process Regression (GPR)
* Kalman Filtering
* Cubic / B-spline interpolation

### ✔ Optimization & Evaluation

* Hyperparameter tuning with Optuna
* Cross-validation
* Loss-surface visualization
* MSE / MAE / RMSE comparison across dozens of GRB IDs

### ✔ Documentation & Manuscript Contribution

* Prepared detailed plots, recorded performance metrics, and contributed text and figures to the collaborative draft.

---

## 🧠 Model Pipeline Summary

### 🔹 Classical Stage

* Spline interpolation
* Gaussian Processes
* Kalman filters

### 🔹 Machine Learning

* k-NN regression
* Polynomial & piecewise regressors

### 🔹 Deep Learning

* LSTM / GRU sequence models
* **Bidirectional LSTM** for dual-direction temporal context
* Transformer encoders for long-range dependencies
* Autoencoders for noise reduction

### 🔹 Hybrid Models

* CNN feature extractor + LSTM decoder
* Kalman residual correction applied to DNN outputs

---

## 📂 Repository Structure

```
GRB-LightCurve-Reconstruction-NAOJ/
│
├── code/
│   ├── lstm_template.ipynb
│   ├── bilstm_template.ipynb
│   ├── gru_template.ipynb
│   ├── gp_regression_template.ipynb
│   └── placeholder.txt
│
├── datasets/
│   └── placeholder.txt
│
├── plots/
│   └── placeholder.txt
│
├── results/
│   └── placeholder.txt
│
└── report/
    └── Internship_Report_Placeholder.pdf
```

*(Folders include placeholders until original files are recovered.)*

---

## 📝 Internship Report

The complete detailed report, code summaries, and model comparisons are included in the `/report/` directory (placeholder added for now).

---

## 🤝 Acknowledgements

I sincerely thank **Prof. Maria Giovanna Dainotti** for her guidance, mentorship, and support throughout this project. Her expertise in GRB astrophysics and machine learning made this internship a transformative learning experience for me.

---

## ⭐ Future Plans

* Re-upload lost GRB result files once recovered
* Add new Transformer-based reconstructions
* Extend GRB forecasting to prompt + afterglow multi-band models
* Publish a cleaned dataset wrapper for reproducible training
