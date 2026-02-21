# LT8390 Synchronous 4-Switch Buck-Boost Converter (12V Output)

This repository contains the design files for a high-efficiency voltage regulator based on the **LT8390EFE**. The board is designed to provide a stable **12V output** from a wide input voltage range (**13V - 60V**), making it ideal for automotive, industrial, and battery-powered applications where the input voltage can be higher or lower than the desired output.


## 🛠 Features
* **Controller:** Analog Devices (Linear Tech) LT8390.
* **Topology:** Synchronous 4-switch Buck-Boost (provides seamless transitions between modes).
* **Input Voltage Range:** 13V to 60V DC.
* **Output Voltage:** Fixed 12V DC.
* **Efficiency:** High-efficiency synchronous rectification using low $R_{DS(on)}$ MOSFETs.
* **Design Tool:** Created with **KiCad 9.0**.
* **Form Factor:** Compact PCB with optimized thermal management and power paths.
<img width="1723" height="1012" alt="image" src="https://github.com/user-attachments/assets/83d3b030-501f-47cc-bb7a-8b27d6484c87" />

## 🔌 Hardware Highlights
* **Power Stage:** Utilizes four external N-channel MOSFETs for maximum current capability and efficiency.
* **Integrated Protection:** Includes input undervoltage lockout (UVLO) and soft-start functionality.
* **Thermal Design:** Large copper pours and thermal vias are implemented to manage heat dissipation from the inductor and MOSFETs.
* **EMI Optimization:** Provision for spread spectrum frequency modulation (SSFM) to reduce EMI signatures.

## ⚙️ Technical Specifications
| Parameter | Value |
| :--- | :--- |
| **Input Voltage ($V_{IN}$)** | 13V - 60V |
| **Output Voltage ($V_{OUT}$)** | 12V |
| **Switching Frequency** | Set via RT resistor (refer to schematic) |
| **Inductor** | High-current shielded power inductor |
| **Input Capacitance** | High-voltage electrolytic + ceramic decoupling array |


## 🚀 Potential Applications
* **Automotive Power:** Stable 12V rail for electronics from a fluctuating 24V/48V vehicle bus.
* **Battery Regulation:** Maintaining 12V from a discharging high-voltage battery pack (e.g., 10S-14S Li-ion).
* **Industrial Control:** Wide-input 24V/48V DC-DC conversion for sensitive sensors.
* **Solar Power:** Regulation of variable solar panel outputs to a fixed 12V battery charging rail.

---
*Note: This project involves high-current power electronics. Ensure proper cooling and current-limit testing during initial bring-up.*
