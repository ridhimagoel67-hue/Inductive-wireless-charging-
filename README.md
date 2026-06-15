# Inductive Power Charging System Simulation using LTspice

## Overview

This project presents the simulation of a **Wireless Power Transfer (WPT)** system using **inductively coupled resonant circuits** in LTspice. Energy is transferred wirelessly from the transmitter coil to the receiver coil through magnetic coupling.

The design demonstrates the principles behind wireless charging technologies used in smartphones, electric vehicles, and IoT devices.

---

## Circuit Components

| Component | Value/Part Number | Function |
|-----------|------------------|----------|
| AC Source | SINE(0 40 100k) | Generates 100 kHz AC signal |
| L1 | 470 µH | Transmitter coil |
| L2 | 470 µH | Receiver coil |
| K1 | 0.95 | Magnetic coupling coefficient |
| C2 | 5.6 nF | Primary resonant capacitor |
| C3 | 5.6 nF | Secondary resonant capacitor |
| D1 | MBRS1100 | Schottky rectifier diode |
| C1 | 100 µF | Output filter capacitor |
| R1 | 100 Ω | Load resistor |

---

## Working Principle

1. The AC source excites the transmitter coil (**L1**) at **100 kHz**.
2. Capacitors **C2** and **C3** create resonant LC tanks that maximize power transfer efficiency.
3. Energy is transferred wirelessly through magnetic coupling (**K = 0.95**) between the coils.
4. The received AC signal is rectified by the Schottky diode (**D1**).
5. The output capacitor (**C1**) smooths the rectified voltage before supplying the load (**R1**).

---

## Simulation Parameters

- Operating Frequency: **100 kHz**
- Coupling Coefficient: **0.95**
- Coil Inductance: **470 µH**
- Resonant Capacitors: **5.6 nF**
- Transient Analysis: **20 µs**

---

## Applications

- Wireless smartphone charging
- Electric vehicle charging
- Biomedical implants
- Consumer electronics
- IoT devices and sensors

---

## Conclusion

This LTspice simulation demonstrates the fundamentals of wireless power transfer using resonant inductive coupling. The circuit highlights efficient energy transfer, AC-to-DC conversion, and output filtering techniques commonly used in modern wireless charging systems.
