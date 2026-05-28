# ESP32 Modular DIN Rail Controller for ESPHome

This repository contains PCB schematics and PCB design files for a modular ESP32-based controller designed for use with ESPHome.

The controller supports expansion modules that provide additional functionality such as extra GPIO, PWM outputs, relays, and other peripherals.

---

## Features

- ESP32-based controller
- Designed for ESPHome
- Modular expansion system
- DIN rail mount enclosure
- Easy integration with custom modules

---

## Supported Expansion Modules

Examples of supported modules:

- GPIO expanders
- PWM output modules
- Relay modules
- Analog input modules
- Custom extension boards

---

## Enclosure Parameters (Fusion 360)

| Parameter | Value |
|---|---|
| Enclosure type | `RailEnclosure_One_Side` |
| Board width | `45 mm` |

---

## Project Structure

```text
/pcb            -> PCB design files
/schematics     -> Electrical schematics
/fusion360      -> Enclosure and mechanical design
/docs           -> Documentation
```

---

## Software

The controller is designed to work with ESPHome firmware.

ESPHome allows easy integration with Home Assistant and other home automation systems.

More information:
https://esphome.io/
