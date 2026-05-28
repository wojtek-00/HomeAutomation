# Sprinkler Expander Module

## Overview

The **Sprinkler Expander Module** is a modular extension board designed for an ESP32-based controller system used with ESPHome home automation projects.

It provides additional digital I/O capabilities as well as flexible power handling for relay-driven actuator systems.

---

## Features

- 8× relay outputs
- 8× digital inputs
- Modular design for sprinkler and automation systems
- Power distribution system with configurable relay supply
- Designed for integration with ESP32 System Controller

---

## Power Architecture

The module contains two independent power domains:

### 1. Logic Power (5V system supply)

- Onboard **bridge rectifier**
- Used to convert optional **AC input into DC**
- Followed by a **5V buck converter**
- Supplies power for:
  - Relay coils
  - ESP32 System Controller (optional power path)

> This allows the system to be powered either from AC or DC sources.

---

### 2. Relay Power Domain

Relay outputs are powered separately from the logic section.

- Default supply: **24VAC (or equivalent external supply)**
- Each relay bank can be powered from a shared rail

#### Individual relay isolation

Each relay channel can be electrically isolated from the main relay power rail by removing a **jumper**.

This allows:
- independent relay supply per channel
- mixed-voltage operation
- custom actuator voltage per output

---

## System Behavior

- Logic section is always powered via 5V rail
- Relay coils may be powered from:
  - shared 24VAC rail (default mode)
  - or independent external supply per channel (jumper removed)

---

## Application

Typical applications:

- Irrigation / sprinkler control systems
- Valve actuation systems
- Distributed relay automation
- Mixed-voltage industrial control logic

---

## Integration

Designed for use with:

- ESP32 System Controller (ESPHome firmware)
- Modular expansion architecture
- DIN rail mounted enclosures

---

## Notes

- Ensure correct jumper configuration before applying relay power
- Do not mix AC and DC relay supply on the same channel
- Verify coil voltage compatibility before deployment
