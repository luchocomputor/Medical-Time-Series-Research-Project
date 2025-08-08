# Spectro-Temporal Causality Analysis in Medical Time-Series

This repository contains the research code and methodological developments for the project *“Spectro-Temporal Granger Causality in EEG/ECG Time-Series”*, conducted from November 2024 to August 2025 in collaboration with CNRS and the Max Planck Institute.

## 📌 Project Summary

We develop and validate a novel framework for time–frequency Granger causality analysis in multivariate biomedical signals. Our goal is to uncover causal interactions between cortical (EEG) and autonomic (ECG) activity during sleep, using high-resolution clinical data.

The proposed approach combines:
- Wavelet-based spectral decomposition,
- Multivariate Vector Autoregressive (VAR) modelling,
- Temporal and spectral formulations of Granger causality,
- Advanced time–frequency visualization tools.

This project contributes to the study of brain–heart dynamics, sleep architecture, and possibly sleep-related pathologies (e.g. sleep apnea) through causal inference.

## 🧠 Data

We use full-night polysomnographic recordings from the **PhysioNet MGH Sleep Lab 2018** database. Each file contains:
- EEG (F3, F4, C3, C4, O1, O2),
- ECG,
- Respiration,
- SaO2,
- Sleep stage annotations (every 30 seconds).

## ⚙️ Methods

- **Preprocessing**: bandpass filtering (0.1–40 Hz), artifact rejection, stationarity testing (ADF/KPSS).
- **VAR Modelling**: model order selection via AIC/BIC, fitted on 40s stationary windows.
- **Granger Causality**:
  - Temporal: using prediction error reduction,
  - Spectral: Geweke's decomposition over frequency bands,
  - Time–frequency: wavelet-based nonparametric estimation.
- **Causal Metrics**: directional, instantaneous, and total causality matrices.
- **Visualisation**: causality scalograms, spectral maps, and phase-specific causal networks.

## 🧾 Publications

- First author of the poster presented at **ISINP 2025 – International Summer Institute on Network Physiology**, held at the Lake Como School for Advanced Studies (Como, Italy) from July 27 to August 1, 2025. The event was organised by the Alessandro Volta Foundation, supported by the W. M. Keck Foundation and Frontiers journal, and directed by Prof. Plamen Ch. Ivanov (PhD, Harvard Medical School & Boston University).
https://isinp.github.io/isinp-4/

- Journal article currently under review in **Frontiers in Network Physiology**, as first author, in collaboration with fellow students, CNRS and École des Ponts researchers, and a PhD candidate from the Max Planck Institute.

