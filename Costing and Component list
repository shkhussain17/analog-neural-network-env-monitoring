# Component List & Costing

Complete Bill of Materials (BOM) for the Analog Multi-Sensor Environmental Monitoring & Safety System, including Layer 1 (sensor neurons) and Layer 2 (decision logic).

## Layer 1 — Sensor Neurons

| Component | Qty | Purpose | Approx Cost (₹) |
|---|---|---|---|
| TL084 (Quad JFET Op-Amp) | 2 | Comparator neurons (8 channels needed) | 40 – 70 |
| NTC Thermistor 10kΩ | 3 | Humidity (wet+dry pair) + Temperature | 30 – 60 |
| LDR | 1 | Light sensing | 10 – 20 |
| MQ2 Gas Sensor Module | 1 | Gas/smoke concentration sensing | 60 – 90 |
| Potentiometer 10kΩ | 8 | Threshold/reference setting per neuron | 80 – 160 |
| Resistor 10kΩ | 8 | Voltage dividers + feedback | 8 – 16 |
| Resistor 100kΩ | 5 | Schmitt trigger feedback (hysteresis) | 5 – 10 |
| Resistor 220Ω | 5 | LED current limiting (pre-transistor stage) | 5 – 10 |
| LED (5mm, mixed colors) | 5 | Neuron status indicators | 10 – 25 |

**Layer 1 Subtotal: ₹248 – ₹461**

## Layer 2 — Decision Logic

| Component | Qty | Purpose | Approx Cost (₹) |
|---|---|---|---|
| BC547 NPN Transistor | 4 | Output drivers (Alarm, Fan, Ventilation) + NOT gate | 12 – 20 |
| 1N4148 Diode | 5 | AND gate (×2) + OR gate (×3) | 10 – 15 |
| Resistor 10kΩ | 6 | Base resistors + pull-downs | 6 – 12 |
| Resistor 470Ω – 680Ω | 4 | LED current limiting (post-transistor, corrected value) | 4 – 8 |
| LED / Buzzer / Relay module | 4 | Final outputs (Alarm, Exhaust Fan, Ventilation, All Clear) | 40 – 120 |

**Layer 2 Subtotal: ₹72 – ₹175**

## Power & Prototyping

| Component | Qty | Purpose | Approx Cost (₹) |
|---|---|---|---|
| 9V Battery | 1–2 | Power supply | 20 – 80 |
| Battery Connector/Snap | 1–2 | Battery interface | 10 – 30 |
| Switch (SPST) | 1 | Main power switch | 10 – 20 |
| Breadboard (full size) | 1–2 | Prototyping | 80 – 160 |
| Jumper Wires (set) | 1 | Connections | 40 – 60 |
| Soft Cloth + Rubber Holder | — | Wet NTC humidity setup | 10 – 20 |

**Power & Prototyping Subtotal: ₹170 – ₹370**

## Grand Total (Breadboard Prototype Stage)

**₹490 – ₹1,006 approx**

## Optional — PCB Version

| Item | Approx Cost (₹) |
|---|---|
| PCB Fabrication (JLCPCB, 5 pcs) | 300 – 600 |
| Soldering consumables (flux, solder wire) | 50 – 100 |
| Header pins/connectors | 30 – 60 |

**PCB Extra: ₹380 – ₹760**

---

## Notes

- All resistor/potentiometer values are tuned during calibration in Falstad simulation before finalizing on hardware.
- MQ2 requires a warm-up period (~20–60 seconds) after power-on for stable readings.
- Prices are approximate, based on robu.in and may vary by vendor.
