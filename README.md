# Real-Time EV Battery Management System

## Project Overview

This project focuses on developing a real-time Electric Vehicle
Battery Management System (BMS) using ESP32.

The system is developed and tested using the Wokwi simulation
environment.

The BMS progressively implements battery monitoring, State of
Charge estimation, fault detection, protection and real-time
visualization.

---

## Project Objectives

- Monitor battery voltage
- Monitor battery current
- Monitor battery temperature
- Estimate State of Charge (SOC)
- Detect battery faults
- Provide visual and audible warnings
- Implement battery protection logic
- Display real-time battery information
- Develop a real-time monitoring dashboard

---

## Development Stages

| Stage | Description | Status |
|---|---|---|
| Stage 1 | Voltage and Temperature Monitoring | Completed |
| Stage 2 | Current Monitoring and SOC | In Progress |
| Stage 3 | Fault Detection | Planned |
| Stage 4 | Protection System | Planned |
| Stage 5 | Cell Monitoring | Planned |
| Stage 6 | Data Logging | Planned |
| Stage 7 | Real-Time Dashboard | Planned |

---

# Stage 1

## Features

Stage 1 implements:

- Battery voltage monitoring
- Temperature monitoring
- OLED display
- Fault detection
- Green status LED
- Red fault LED
- Buzzer alarm

## Hardware

- ESP32 DevKit
- SSD1306 OLED
- Potentiometer
- DS18B20
- Green LED
- Red LED
- Buzzer
- 220 ohm resistors

## Pin Configuration

| Component | Pin |
|---|---|
| Battery Voltage | GPIO34 |
| Temperature | GPIO4 |
| OLED SDA | GPIO21 |
| OLED SCL | GPIO22 |
| Green LED | GPIO26 |
| Red LED | GPIO27 |
| Buzzer | GPIO14 |

## Simulation

The project is developed using Wokwi.

The potentiometer simulates battery voltage while the DS18B20
simulates battery temperature.

## Stage 1 Status

Stage 1 has been successfully implemented and tested.

---

# Future Development

Stage 2 will introduce:

- Current measurement
- Charging/discharging detection
- Real-time SOC estimation

Later stages will introduce advanced fault detection,
protection, cell monitoring, data logging and dashboard
visualization.

---

## Disclaimer

This project is an educational/simulation implementation.
The Wokwi potentiometer represents simulated sensor input and
does not constitute an automotive-rated battery monitoring
system for use with a real high-voltage EV battery pack.
