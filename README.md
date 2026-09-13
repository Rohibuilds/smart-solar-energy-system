<div align="center">

# Smart Solar Energy System

**ESP32 solar-storage monitor with INA219 sensing, battery estimation and a real-time web dashboard.**

![Status](https://img.shields.io/badge/status-working_prototype-00D9A5?style=flat-square)
![Platform](https://img.shields.io/badge/platform-ESP32_%C2%B7_IoT-101820?style=flat-square)
![Brand](https://img.shields.io/badge/by-RA_TECH-101820?style=flat-square)

</div>

## Overview

An ESP32-based energy monitor for a small solar storage and fast-charge system. It measures voltage, current, and power through an INA219 and presents the data on a clean phone-friendly web dashboard.

> **Project status:** Working prototype

## Highlights

- Live voltage, current, and power monitoring
- Estimated battery percentage
- Responsive ESP32 web dashboard
- Solar charging and dual-cell storage workflow
- Fast-charge output stage
- Correct INA219 high-side measurement orientation

## Hardware

| Component | Role |
|---|---|
| ESP32 development board | Main processing and control |
| INA219 current and voltage sensor | Project subsystem |
| Two 18650 cells with suitable protection | Project subsystem |
| Two 6 V solar panels | Project subsystem |
| XL6009 boost converter | Project subsystem |
| Buck converter | Project subsystem |
| MH-KC24 fast-charge module | Project subsystem |

## Repository structure

```text
smart-solar-energy-system/
├── firmware/   Tested source code and configuration notes
├── hardware/   Wiring, components, PCB, and enclosure information
├── docs/       Build guide, calibration, results, and troubleshooting
├── media/      Prototype images, diagrams, and demo links
└── README.md   Project overview and release status
```

## Current public release

This initial release establishes the verified project overview and a clean documentation structure. Firmware, wiring diagrams, and media will be added only after each item is checked for accuracy and private credentials are removed.

## Roadmap

- [ ] Publish the final tested firmware
- [ ] Add a complete power-flow diagram
- [ ] Document calibration and battery-safety checks
- [ ] Add dashboard screenshots and measured efficiency results

## Safety and reproducibility

- Verify every supply voltage before powering the controller or modules.
- Use a common ground and a power source sized for peak motor or audio current.
- Never commit Wi-Fi passwords, API keys, personal contact details, or certificates.
- Recheck the published pin map against the tested hardware before assembly.

---

<div align="center">

**Designed and developed by [Rohi · RA TECH](https://github.com/Rohibuilds)**

<sub>Build. Test. Improve. Share.</sub>

</div>
