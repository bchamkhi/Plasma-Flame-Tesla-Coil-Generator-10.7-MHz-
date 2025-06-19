# Plasma-Flame-Tesla-Coil-Generator-10.7-MHz-
This is a DIY high-frequency **Plasma Flame Generator** based on a loosely coupled **dual resonant transformer** principle. It uses an IRFP460 MOSFET and feedback coil to self-oscillate and create a stable flame output from a screw electrode on top of the secondary coil.
## ⚙️ Circuit Overview

- Self-oscillating LC driver with IRFP460
- Feedback coil provides automatic gate control
- Series-tuned primary coil
- Loosely coupled secondary for plasma output

---

## 🔩 Components List

| Ref | Component             | Value / Type         | Notes                                     |
|-----|-----------------------|----------------------|-------------------------------------------|
| Q1  | N-MOSFET              | IRFP460              | High-speed, high-voltage switch           |
| C1  | Resonant Capacitor    | 4.7 nF / 2 kV         | Pulse-rated                               |
| C2+C3 | Parallel Capacitors | 2 × 33 nF K15V        | Across primary                            |
| R1  | Gate Resistor         | 1 kΩ / 1 W            | Gate–Source                               |
| R2  | Potentiometer Resistor | 1 kΩ / 5 W          | In series with RV1                        |
| RV1 | Potentiometer         | 100 kΩ (or 10 kΩ)     | Feedback control                          |
| D1  | Zener Diode           | 12 V                  | Across potentiometer                      |
| D2  | TVS Diode             | 1.5KE15CA             | Gate protection                           |
| C4  | Filter Capacitor      | 10 µF / 400 V         | Power filtering                           |
| PWR | DC Supply             | 12–40 V, ≥5 A         | Power input                               |

---

## 🧲 Coil Specifications

| Ref | Coil       | Description |
|-----|------------|-------------|
| L1  | Secondary  | 0.5 mm wire, 124 turns, 32 mm PVC, 62 mm height. Screw electrode (6 mm × 11 mm) on top. |
| L2  | Primary    | 1.2 mm wire, 10 turns on 52 mm PVC. Best resonance at ~7 turns. Spaced ~1.5 mm. |
| L3  | Feedback   | 18 AWG jumper wire, 13.5 turns, 32 mm tube. Connected to MOSFET Gate. |

---

## 🔬 Resonance & Operation

- **Resonant Frequency (measured):** ~10.7 MHz
- **Effective Capacitance:** ≈ 4.39e-09 F
- **Primary Inductance:** ≈ 1.45e-05 H
- **Theoretical Frequency:** ≈ 0.63 MHz

📌 Actual frequency is higher due to coupling, feedback stabilization, and layout effects. Flame confirms real resonance.

---

## 💡 Tuning Notes

- Adjust primary (L2) turns from 10 down to 7 for best output.
- Use oscilloscope or flame length for fine tuning.
- Feedback ensures self-locking resonance.

---

## ⚠️ Safety

⚡ High-frequency, high-voltage plasma is dangerous.  
Use proper insulation, protection, and operate only in safe environments.

---

## 📁 Project Structure

```
plasma_flame_tesla_coil/
├── README.md
├── LICENSE
├── images/
├── schematics/
```

---

## 📜 License

MIT License – Free to use, modify, and share.
