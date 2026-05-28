# HomeAutomation

A modular home automation system built around ESPHome, custom PCB design (KiCad), and 3D-printed enclosures.

The project is designed to be **scalable**, allowing multiple independent hardware modules (controller + expanders) that integrate into a single automation system.

---

# 🧠 System Overview

The project is split into two main domains:

## 🧩 hardware/
Contains all physical devices and their design artifacts:

- PCB designs (KiCad)
- 3D enclosures (STEP / CAD files)
- front panels / UI elements
- production-ready snapshots (releases)

Each hardware module is self-contained.

### Current modules:
- `system_controller` – main brain of the system
- `relay_expander` – relay output module (8 outputs + 8 inputs)
- *(future expanders will be added here)*

---

## ⚙️ system/
Contains software and logic:

- ESPHome configurations
- automation logic (e.g. Home Assistant)
- device behavior definitions
- shared system-level configuration

This layer defines **how devices behave**, not how they are built.

---

# 🏗️ Hardware Module Structure

Each hardware module follows the same structure:
 - hardware/<module_name>/
 - current/ # active development (WIP)
 - releases/ # frozen production versions
