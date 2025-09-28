# CircuitPython LoRa RX / TX

Code originally created by Dygear (https://github.com/Dygear)
---
This project demonstrates LoRa communication using **CircuitPython** on the [Adafruit Feather RP2040](https://www.adafruit.com/product/4884) with the [RFM95 LoRa Radio (915 MHz)](https://www.adafruit.com/product/3072) — RadioFruit edition with STEMMA QT support.  

It includes both **transmitter (TX)** and **receiver (RX)** examples. The transmitter setup integrates GPS data using the [Adafruit Ultimate GPS FeatherWing (PA1616D)](https://www.adafruit.com/product/3133), allowing location information to be sent over LoRa.  

---

## Hardware Used
- [Adafruit Feather RP2040](https://www.adafruit.com/product/4884)  
- [Adafruit RFM95 LoRa Radio - 915 MHz - RadioFruit with STEMMA QT](https://www.adafruit.com/product/3072)  
- [Adafruit Ultimate GPS FeatherWing - PA1616D](https://www.adafruit.com/product/3133) (for TX setup)  

---

## Features
- LoRa **transmit (TX)** and **receive (RX)** examples.  
- GPS integration on TX side (latitude, longitude, and more).  
- CircuitPython-based for easy prototyping and customization.  
- STEMMA QT compatible for quick sensor expansion.  

---

## CircuitPython Setup
1. Install the latest version of [CircuitPython](https://circuitpython.org/board/feather_rp2040/) on your Feather RP2040.  
2. Copy the required libraries from the [Adafruit CircuitPython Bundle](https://circuitpython.org/libraries).  
   - `adafruit_rfm9x.mpy`  
   - `adafruit_bus_device`  
   - `adafruit_gps.mpy` (for TX setup)  
   - `adafruit_logging.mpy` (optional, for debug output)  
3. Upload the `code.py` file (or `tx_code.py` / `rx_code.py`) to your board.  

---

## Wiring Notes
- The Feather RP2040 connects directly with the RFM95 via SPI.  
- The GPS FeatherWing stacks onto the Feather for TX setup.  
- STEMMA QT port is available for additional sensors if needed.  

---

## Usage
- **TX Mode:** Sends GPS data (or test strings if GPS not fixed) over LoRa.  
- **RX Mode:** Listens for LoRa packets and prints received messages to the REPL/serial console.  


