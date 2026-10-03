# Stage 1 - Battery Voltage and Temperature Monitoring

## Objective

The objective of Stage 1 is to develop the basic monitoring section
of a real-time Electric Vehicle Battery Management System (BMS).

The ESP32 continuously monitors:

- Battery voltage
- Battery temperature

The measured information is displayed on an OLED screen.

## Hardware

- ESP32 DevKit
- SSD1306 128x64 OLED
- Potentiometer for simulated battery voltage
- DS18B20 temperature sensor
- Green LED
- Red LED
- Buzzer
- 220 ohm resistors

## Pin Configuration

| Component | ESP32 Pin |
|---|---|
| Battery potentiometer SIG | GPIO34 |
| DS18B20 DATA | GPIO4 |
| OLED SDA | GPIO21 |
| OLED SCL | GPIO22 |
| Green LED | GPIO26 |
| Red LED | GPIO27 |
| Buzzer | GPIO14 |

## Battery Voltage Simulation

The potentiometer is used to simulate the battery voltage.

0 V ADC input represents approximately 6.0 V battery voltage.

3.3 V ADC input represents approximately 8.4 V battery voltage.

## Temperature Monitoring

The DS18B20 continuously measures the simulated battery temperature.

The system considers temperatures outside the configured limits
as a fault condition.

## Fault Detection

The system detects:

- Low battery voltage
- High battery voltage
- Low temperature
- High temperature

## Indication

### Normal

- Green LED ON
- Red LED OFF
- Buzzer OFF
- OLED displays NORMAL

### Fault

- Green LED OFF
- Red LED ON
- Buzzer ON
- OLED displays FAULT

## Stage 1 Result

Stage 1 successfully demonstrates basic real-time battery
voltage and temperature monitoring using ESP32.
