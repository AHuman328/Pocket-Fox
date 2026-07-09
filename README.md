# Pocket-Fox

*A portable cybersecurity research platform for security professionals, students, researchers, and hardware enthusiasts.*

## Overview

Pocket-Fox is an all-in-one handheld cybersecurity research platform that combines the capabilities of multiple portable security tools into a single modular device.

Rather than replacing any one existing platform, Pocket-Fox draws inspiration from several established projects and combines their ideas into a unified hardware and software ecosystem focused on research, education, and authorized security testing.

Inspirations include:

* Flipper Zero
* HackRF One
* WiFi Pineapple
* ESP32 Marauder
* Cyberdecks
* Pwnagotchi

The long-term goal is a compact handheld platform — approximately **6 × 8 × 1.5 inches** — capable of supporting a wide range of security research workflows, while remaining fully documented and reproducible.

---

## Goals

Pocket-Fox is being developed to provide:

* A portable cybersecurity research platform
* Modular hardware expansion
* Embedded systems experimentation
* Wireless research capabilities
* A customizable Linux-based software environment
* Comprehensive documentation for builders and developers

---

## Intended Users

Pocket-Fox is intended for:

* Cybersecurity students
* Security researchers
* Authorized penetration testers
* Makers
* Hardware enthusiasts
* Embedded systems developers

---

# Hardware Concept

Pocket-Fox is built around a hybrid architecture: a Linux-based embedded computer paired with dedicated microcontrollers for specialized hardware tasks.

## Main Processing System

### Orange Pi Zero 3 (4GB)

The Orange Pi serves as the primary computing platform, responsible for:

* Running the custom Linux operating system
* Managing the touchscreen user interface
* Storage and application execution
* Coordinating communication between onboard peripherals
* Executing user-installed applications and research tools

---

## Auxiliary Controllers

### Dual ESP32-S3 Super Mini

Two dedicated ESP32-S3 microcontrollers offload peripheral management from the Orange Pi, keeping the Linux system responsive while time-sensitive embedded tasks run independently.

**ESP32 #1**
Handles radio-related peripherals and wireless hardware interfaces.

**ESP32 #2**
Handles sensors, physical controls, GPS, LEDs, power monitoring, and future expansion peripherals.

---

## Display & Controls

Pocket-Fox is designed around:

* **4.3-inch IPS Capacitive Touch Display**
  * 800 × 480 resolution
  * HDMI interface
* Directional pad (D-pad)
* Navigation buttons
* Additional programmable function buttons

Physical controls keep the device fully usable even when touchscreen interaction isn't convenient.

---

## Wireless Hardware

Current hardware planning includes:

* Wi-Fi
* Bluetooth
* GPS
* Sub-GHz radio support
* Optional future LoRa expansion

Wireless hardware is distributed across dedicated subsystems to improve modularity and simplify future upgrades.

---

## Additional Hardware

Planned supporting hardware includes:

* NFC
* RFID
* Infrared transceiver
* Internal battery management system
* USB connectivity
* Expansion interfaces for future modules

Additional components may change as development progresses.

---

## Power System

Current design targets include:

* 7500 mAh single-cell LiPo battery
* USB-C charging circuitry
* Regulated power rails for both the Linux system and embedded subsystems
* Battery monitoring and protection

The final power architecture will be refined during hardware prototyping.

---

## Enclosure

Pocket-Fox is planned around a custom 3D-printed enclosure with a target size of:

**6 × 8 × 1.5 inches**

The enclosure is being designed to maximize portability while still allowing internal access for servicing and future revisions.

---

## Current Development Status

Pocket-Fox is currently in the planning and architecture phase.

* ✅ Initial hardware concept
* ✅ Repository redesign
* ✅ System architecture planning
* 🚧 Component evaluation
* ⏳ Prototype development
* ⏳ PCB design
* ⏳ Custom Linux environment

---

# Design Philosophy

Pocket-Fox is built around three core principles.

## Portability

A complete cybersecurity research environment designed to travel anywhere.

## Expandability

Every major subsystem is designed with future hardware and software expansion in mind.

## Documentation

Every stage of development — from initial planning through final assembly — will be documented, making the project reproducible for builders, contributors, and future developers.

---

## Disclaimer

Pocket-Fox is intended for cybersecurity education, hardware experimentation, research, and **authorized** security testing only. Users are responsible for ensuring they have permission before interacting with any network, system, or device.
