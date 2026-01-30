# 4-Level Water Level Indicator (Digital Logic Design)

> "A digital logic circuit design for a 4-level water indicator using logic gates (AND/OR) with cumulative LED outputs and a buzzer alarm."

---

## 📋 Project Overview
This project focuses on designing and implementing a digital logic circuit that acts as a **4-level water indicator**. The system is built using pure combinational logic, avoiding the use of microcontrollers like Arduino to demonstrate core hardware logic principles.

## 🚀 System Features
* **Sensor Inputs:** 4 conductive wires (W1, W2, W3, W4) placed at different heights in a tank.
* **Cumulative Outputs:** LEDs (L1, L2, L3, L4) turn on sequentially and stay on as the water level rises.
* **Alert System:** A buzzer is integrated with the highest water level (L4) to indicate a full tank.

## 🧠 Logic Design & Equations
The circuit logic was derived from a comprehensive truth table and simplified using **Karnaugh Maps (K-Maps)** to achieve the most efficient gate count.

### Boolean Equations:
* **L1 (Level 1):** $L1 = W1 + W2 + W3 + W4$
* **L2 (Level 2):** $L2 = W1 \cdot W2 + W3 + W4$
* **L3 (Level 3):** $L3 = W1 \cdot W2 \cdot W4 + W3$
* **L4 (Level 4/Buzzer):** $L4 = W1 \cdot W2 \cdot W3 \cdot W4$

## 🛠️ Implementation
The project includes a Breadboard Simulation using the following Integrated Circuits (ICs):
* **74HC08:** Quad 2-input AND gates.
* **74HC32:** Quad 2-input OR gates.

### Visual Documentation & Downloads
![Simulation Circuit](Water-level-indicator-simulation.png)

📄 **Technical Files:**
* [Download Schematic PDF](Water-level-indicator-schematic.pdf)

---
