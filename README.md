# RF Class-A Power Amplifier Design & PCB Layout

A single-stage BJT-based Class-A Power Amplifier operating in the **400 MHz – 500 MHz** frequency band, designed, simulated, and translated into a custom printed circuit board layout using **Altium Designer**.

---

## 📌 Project Overview

This project demonstrates the complete end-to-end hardware design flow of a high-gain RF Class-A power amplifier, encompassing schematic capture, DC biasing configuration, RF matching networks, and full production-ready PCB layout implementation in Altium Designer. The layout focuses on maintaining high signal integrity, controlled impedance traces, and optimal thermal/ground stability for high-frequency operations.

---

## ⚡ Key Circuit Specifications & Features

* **Topology:** Single-stage BJT (NPN) Class-A Amplifier using the **BFR93A** transistor.
* **Operating Frequency Range:** 400 MHz – 500 MHz.
* **Supply Voltage ($V_{cc}$):** 10 V DC.
* **Biasing Scheme:** Stable voltage-divider DC biasing network ensuring a continuous $360^\circ$ conduction angle.
* **Impedance Matching:** Input ($L_2, C_4, C_5$) and output ($L_3, C_2$) LC matching networks optimized for $50\,\Omega$ port impedances.
* **Interconnects:** High-frequency SMA edge-launch connectors ($J_1, J_2$) for accurate laboratory testing and network analyzer interfacing.

---

## 📐 Schematic & Circuit Design

The schematic was designed to handle high-frequency AC signals while maintaining stable DC operating points. It integrates decoupling capacitors, feedback components, and precise matching stages around the active BFR93A device.

---

## 🖨️ PCB Layout & Implementation (Altium Designer)

The layout was engineered to minimize parasitics and high-frequency signal degradation at RF frequencies:

* **Controlled Impedance:** Routed 50-ohm microstrip transmission lines connecting the SMA edge-launch connectors to the matching networks to minimize reflection coefficients ($S_{11}, S_{22}$).
* **Ground Management:** Integrated solid ground planes with strategic thermal via stitching around component pads and active device pins to suppress stray inductances and ensure structural RF stability.
* **Component Placement:** Minimized trace lengths for critical matching elements ($L_2, L_3, C_2, C_4$) to reduce stray series inductance and shunt capacitance.

### Design Previews

**Schematic Design**
<img width="920" height="507" alt="image" src="https://github.com/user-attachments/assets/7b44a39f-e106-4995-88e6-4d9c2c6903ee" />
<br>**2D PCB Layout**
<img width="1295" height="683" alt="image" src="https://github.com/user-attachments/assets/b42af9dd-f179-464d-82ad-d27c636002ac" />
<br>**3D Board Visualization**
<img width="1293" height="517" alt="image" src="https://github.com/user-attachments/assets/bf3036df-22cc-45b2-bced-010d724dfad3" />

---

## 🛠️ Software Tools Used

* **Altium Designer** – Schematic capture, component footprint management, 2D PCB layout routing, and 3D enclosure/board visualization.
