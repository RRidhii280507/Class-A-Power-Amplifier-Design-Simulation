# Class-A Power Amplifier Design & Simulation

A single-stage BJT-based Class-A Power Amplifier operating in the **400 MHz – 500 MHz** frequency band, designed and simulated using **Qucs (Quite Universal Circuit Simulator)**.

---

## 📌 Project Overview
This project demonstrates the schematic design, DC operating point bias configuration, and Small-Signal S-parameter performance analysis of a high-gain Class-A amplifier. The circuit is designed to ensure maximum linear power transfer, minimal input reflection, and high stability across transistor parameter variations.

---

## ⚡ Key Circuit Specifications & Features

* **Topology:** Single-stage BJT (NPN) Class-A Amplifier.
* **Frequency Range:** 400 MHz – 500 MHz (Linear Sweep).
* **Supply Voltage ($V_{CC}$):** 10 V DC.
* **Biasing Scheme:** Voltage-divider bias network ensuring full $360^\circ$ conduction angle.
* **Impedance Matching:** Input and output LC networks optimized for $50\ \Omega$ port impedances ($P_1, P_2$).
* **Simulation Types:** DC Bias Point Simulation, S-Parameter Analysis, and Parameter Sweep on Transistor Beta ($B_f$).

---

## 📐 Circuit Schematic

The complete schematic built in Qucs includes DC biasing, emitter/collector feedback, coupling capacitors, and LC matching stages:

* **Biasing Network:** $R_1 = 2088\ \Omega$, $R_2 = 7192.7\ \Omega$, $R_3 = 125\ \Omega$, $R_c = 500\ \Omega$, $R_{e1} = 50\ \Omega$.
* **Input Matching Network:** $L_1 = 85.27\text{ nH}$, $C_3 = 1.50\text{ pF}$, $C_1 = 10\text{ pF}$.
* **Output Matching Network:** $L_2 = 847.87\text{ nH}$, $C_4 = 232.71\text{ fF}$.

<img width="1487" height="822" alt="image" src="https://github.com/user-attachments/assets/198b6ab8-f324-4307-9e31-2ab506fe4203" />


---

## 📊 Simulation Results

### 1. Small-Signal S-Parameter Performance
* **Forward Gain ($S_{21}$):** Reaches a peak forward transmission gain exceeding **38 dB** in the 400–430 MHz operating window.
* **Input Return Loss ($S_{11}$):** Drops well below **-10 dB** (reaching down to ~**-19.1 dB** at 4.28e8 Hz), indicating excellent input matching to $50\ \Omega$.
* **Output Reflection ($S_{22}$):** Achieves strong impedance match around the target center frequency.

### 2. Parameter Sweep Analysis
A parameter sweep was performed on the transistor forward current gain ($B_f$) ranging from **50 to 250** across 20 linear points to verify circuit robustness and gain sensitivity against manufacturing tolerances.

---

## 🛠️ Software Tools Used
* **Qucs 0.0.19** (Quite Universal Circuit Simulator)

---
