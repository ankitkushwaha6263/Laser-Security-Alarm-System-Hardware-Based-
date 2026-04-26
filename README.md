
# Laser Security Alarm System

A simple yet highly effective hardware-based security system that triggers an alarm when a laser beam is interrupted. This project uses a transistor-based switching logic, making it efficient and easy to build without complex microcontrollers.

---

## 🛠️ Components Required

| Component | Specification | Purpose |
| :--- | :--- | :--- |
| **Transistor** | BC547 (NPN) | Acts as an electronic switch |
| **Sensor** | LDR (Light Dependent Resistor) | Detects the laser beam |
| **Resistor** | 10k Ohm | Pull-up resistor for Transistor Base |
| **Output** | 5V-9V Buzzer | Provides the audible alarm |
| **Laser Source** | 5V Laser Diode | The security beam |
| **Power** | 9V Battery | Power supply for the circuit |

---

## 🔌 Connection Table (Pin-to-Pin)

| From Component | Pin | To Component | Pin |
| :--- | :--- | :--- | :--- |
| **BC547** | Emitter | **Battery** | Negative (-) |
| **BC547** | Base | **LDR** (Pin 1) & **10k Resistor** | Node |
| **10k Resistor** | Other End | **Battery** | Positive (+) |
| **LDR** | Pin 2 | **Battery** | Negative (-) |
| **Buzzer** | Positive (+) | **Battery** | Positive (+) |
| **Buzzer** | Negative (-) | **BC547** | Collector |

---

## ⚙️ Working Principle

The circuit operates on the principle of a **Voltage Divider** and **Transistor Switching**:

1. **Light Condition:** When the laser beam hits the LDR, its resistance becomes very low. This pulls the Base of the BC547 transistor to a low voltage (logic 0). The transistor remains in "OFF" state, and the buzzer stays silent.
2. **Interruption (Dark) Condition:** When someone crosses the beam, the LDR resistance increases instantly. The 10k resistor then pulls the Base voltage high (logic 1). This turns the transistor "ON," allowing current to flow through the buzzer, sounding the alarm.

---

## 🚀 Key Features
* **Zero Latency:** Immediate alarm response.
* **Low Power Consumption:** Runs for a long time on a standard 9V battery.
* **Scalability:** Can be expanded using mirrors to create a 360-degree security perimeter.

---

## 📸 Circuit Diagram
in circiut folder
