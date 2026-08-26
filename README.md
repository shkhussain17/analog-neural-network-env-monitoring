# Analog Multi-Sensor Environmental Monitoring & Safety System

A **microcontroller-free** environmental monitoring and safety system built entirely with analog electronics — op-amp based "artificial neurons," Schmitt trigger noise immunity, and diode/transistor logic gates for real-time decision-making. No code, no CPU — pure analog signal processing.

## Overview

This project explores whether "intelligent" decision-making can be implemented purely through analog circuits instead of software. Inspired by the concept of a neural network, it uses op-amp comparators as artificial neurons — each sensor stage independently makes a threshold-based decision, and these decisions are logically combined to trigger real-world automated responses (alarms, fans, indicators).

## Features

- **4 environmental sensors:** Humidity (wet/dry NTC pair), Temperature (NTC), Light (LDR), Gas concentration (MQ2)
- **5 analog "neurons"** (op-amp comparators) for individual sensor threshold detection
- **Schmitt trigger hysteresis** on every stage — eliminates false triggering from sensor noise
- **Multi-level gas detection** — separate Warning and Danger thresholds (window comparator design)
- **Diode-based logic gates (AND/OR/NOT)** to combine sensor outputs into smart decisions
- **Zero software/microcontroller dependency** — fully analog, low-power, instant response

## System Architecture

### Layer 1 — Sensor Neurons
| Neuron | Sensor | Type |
|---|---|---|
| Temperature | NTC (dry) | Standalone comparator |
| Humidity | NTC (wet) vs NTC (dry) | Differential comparator |
| Light | LDR | Standalone comparator |
| Gas Warning | MQ2 | Standalone comparator (low threshold) |
| Gas Danger | MQ2 | Standalone comparator (high threshold) |

### Layer 2 — Decision Logic
| Output | Trigger Logic |
|---|---|
| Gas Leak Alarm | Gas Danger HIGH |
| Gas Exhaust Fan | Gas Warning HIGH |
| Auto Ventilation | Humidity HIGH **AND** Temperature HIGH |
| All Clear Indicator | No alerts active (OR + NOT logic) |

## Components Used

- TL084 (Quad JFET Op-Amp) — comparator neurons
- BC547 NPN Transistor — output drivers & NOT gate
- 1N4148 Diodes — AND/OR logic gates
- NTC Thermistors ×3, LDR, MQ2 Gas Sensor
- Resistors, Potentiometers (calibration), LEDs

## Tools Used

- **Falstad Circuit Simulator** — circuit design & simulation
- (Planned) Breadboard prototyping and PCB design in KiCad

## Project Status

- ✅ Layer 1 (all 5 sensor neurons) designed and simulated
- ✅ Schmitt trigger noise immunity implemented on all stages
- ✅ Output driver stage (transistor-based) — current-limiting fixed
- 🔲 Layer 2 logic gates (AND/OR/NOT) — in progress
- 🔲 Breadboard hardware prototype
- 🔲 PCB design

## Learning Outcomes

- Practical application of op-amp configurations (comparator, differential amplifier, Schmitt trigger)
- Diode-resistor logic gate design
- Multi-sensor system architecture and signal combination
- Circuit-level noise immunity techniques

## Author

Hussain Mohammadali Shaikh — Electronics & Telecommunication Engineering, Shree L.R. Tiwari College of Engineering

## License

*(Add license if applicable, e.g., MIT)*
