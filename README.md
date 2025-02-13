# 🛰️ Vega - Model Rocket Flight Computer 🚀  

### **A modern, feature-rich flight computer for model rocketry.**  

---

# 📌 Features  
✅ Accelerometer based apogee detection <br>
✅ Adjustable Launch detection<br>
✅ Supports GPS location (using BN-880)<br>
✅ Data Logging via 8MB on board flash<br>
✅ Compatible with Cosmic Tower  <br>
✅ Transmits telemetry via E220-900T22D LoRa module (1Hz)<br>
✅ Supports Thrust Vector Controlled flights  <br>
✅ On board EEPROM for saving flight settings <br>

# 🦺 Safety Features

## ARMING terminal
Pyrotechnics may only be enabled if and only if this terminal is shorted during launch day. It is crucial that this terminal
is not shorted during the debugging stage of the rocket.

## BYPASS terminal
The Pypass terminal will ensure that the rockets main power source is not souly relying on the physical toggle switch. You MUST
properly short this terminal during launch, not doing so WILL cause your rocket to malfunction and have a catastrophic failure.

## CONTINUITY indicators
Underneath each pyrotechnic terminal is an LED which will shine a very bright GREEN light when the terminal has continuity. This visual
queue will let the user know that the pyro channels are LIVE and ready to go. Note that the LEDs can only show continuity if and only if
the ARM terminal is also shorted.

## ACCELEROMETER Based Apogee Detection
Accelerometer based apogee detection will allow for high precision, non-environmental based apogee detection. Unlike barometric apogee detection, which has high noise, and is drastically affected by both light & temperature, the accelerometer based apogee detection only relies on gravity. By taking the magnitude of all 3 axis at any given time, it is almost guaranteed to detect apogee, since only a gravitational acceleration is pulled on the rocket at apogee. (The detection system includes uncertainty such as drift)

## LAUNCH DETECTION
The rocket only enters flight mode if and only if the launch detection parameter is less than the current vertical acceleration of the rocket. The sensitivity (value) of the launch detection can be modified in the Cosmic Tower.

## PARACHUTE DELAY
Using the Cosmic Tower (available on the Microsoft store), the user may change various paramters, this includes an apogee delay in the case the rocket enters high altitudes where the user may want the rocket to freefall. An apogee delay is also useful to ensure the rocket is indeed past apogee and has a lowest speed in order not to damage the shoot or apply stress onto the rocket.

---

## 📋 Specifications  

| Feature           | Details                                  |
|------------------|----------------------------------|
| **Processor**    | STM32F411CEU6               |
| **Sensors**      | BME280 & BMI088  |
| **Storage**      | 8MB Flash & 64KB EEPROM       |
| **Power**        | INPUT: 4-23V to 3.3 & 5V       |
| **Deployment**   | 3 Pyro-Channels, 1 Servo Ejection        |
| **Telemetry**    | E220-900T22D with CT ground Module        |
| **Interfaces**   | USB              |
| **Firmware**     | Programmed in C/C++, .bin for firmware updates  |
| **Power Maximums**     | MAX Total current draw of 12 A for 5V & 3 A for 3.3V terminals |

---

## 📏 Dimensions & Weight  

| Parameter       | Value               |
|----------------|---------------------|
| **Size (Fully Assembled)**       | 90.00 x 54.40 x 27.45 mm |
| **Weight (Without Antenna)**     | 57 grams            |

---
*"Note that this Repository is new and is still under development. Please be patient as more information is soon to come!" - Cosmic Aerospace Technologies*
