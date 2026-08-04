# ⚡ Unipolar Voltage Intensifier Circuit (VIC): QSpice Digital Twin & Mathematical Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](../LICENSE)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![QSpice Verified](https://img.shields.io/badge/Simulator-QSpice-green.svg)](https://www.qorvo.com/design-hub/design-tools/interactive/qspice)

## 📌 Overview

This subfolder contains the verified **QSpice schematic files (`.qsch`)**.

Refer to preprint for the simulation analysis:
https://doi.org/10.5281/zenodo.21775603

---

## 📂 Files Included

* `VIC_4400V_8667Hz_Version1.qsch`: Idealized component baseline model.
* `Screenshot 2026-08-03 235954.png`: QSpice waveform simulation capture.

---

## 🛠️ Key Simulation Parameters

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Primary Inductance ($L_1$)** | $50\,\mu\text{H}$ | Step-up transformer primary |
| **Secondary Inductance ($L_2$)** | $150\,\text{mH}$ | Step-up transformer secondary ($N=54.77$) |
| **Aiding Chokes ($L_3, L_4$)** | $47\,\text{mH}$ each | Coupled in magnetic aiding ($k = -0.99$, total $L_{\text{chokes}} = 187\,\text{mH}$) |
| **Total Secondary Inductance** | $337.06\,\text{mH}$ | Combined transformer + choke inductance |
| **Cell Capacitance ($C_{\text{cell}}$)** | $1\,\text{nF}$ | Stainless steel concentric water cell |
| **Water Resistance ($R_{\text{water}}$)** | $1\,\text{M}\Omega$ | Distilled water cell impedance |
| **Carrier Frequency ($f_r$)** | $8,667\,\text{Hz}$ | Tuned LC tank resonant frequency |
| **Gate Modulation ($f_{\text{gate}}$)** | $100\,\text{Hz}$ | 5ms ON / 5ms OFF burst gating |
| **Peak Cell Voltage** | **4,400 V (4.4 kV)** | Unipolar (+), continuous electrostatic stress |
| **System Power Draw** | **9.94 W** | Total battery power draw |

---

## 💻 How to Run

1. Download and install **QSpice** from [Qorvo](https://www.qorvo.com/design-hub/design-tools/interactive/qspice).
2. Open `VIC_4400V_8667Hz.qsch` inside QSpice.
3. Press **Run (F5)** to execute the transient analysis.


