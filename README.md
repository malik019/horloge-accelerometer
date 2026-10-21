# Ultra-Low-Power ATtiny Motion Clock (Horloge)

A compact, low-power embedded hardware platform featuring an **Microchip ATtiny MCU** integrated with an **STMicroelectronics LIS2DW12 ultra-low-power accelerometer** and **WS2812B-MINI addressable RGB LEDs**. 

This repository houses the complete hardware development lifecycle, from schematic capture and board layout to manufacturing documentation.

## 🛠️ Hardware Specifications & Component Selection
* **Microcontroller:** Microchip ATtiny MCU (optimized for compact footprint and low static power draw).
* **Motion Sensing:** STMicroelectronics LIS2DW12 3-axis accelerometer (selected for its sub-microamp low-power modes and configurable wake-on-motion interrupts).
* **Display / Visuals:** WS2812B-MINI addressable RGB LEDs for custom illumination, animations, or gesture-based feedback.
* **Power Management:** Integrated battery layout interface (CR2032 or similar lithium coin cell support).

## 📂 Repository Architecture
The workspace is organized following standard hardware engineering practices:
* **`/design`** — Primary KiCad project assets containing schematics (`.kicad_sch`), PCB layouts (`.kicad_pcb`), global footprint tables, and specialized local hardware libraries.
* **`/fabrication`** — Production-ready Gerber files, drill plots, and Open Parts List (OPL) Bill of Materials data ready for manufacturing.
* **`/documentation`** — Comprehensive hardware design review documents and exportable schematics in PDF format for immediate evaluation.

## 🚀 Key Engineering Focus Areas
* **Power Optimization:** Leveraged the LIS2DW12 accelerometer's hardware interrupt pins to wake the ATtiny MCU from deep sleep modes, maximizing overall battery runtime.
* **Signal Integrity:** Carefully routed digital signals for the high-speed data lines driving the addressable NeoPixel array while isolating noise near the sensor.
* **Form Factor Constraint:** Designed a dense, highly integrated multi-layer layout tailored for a compact, wearable or portable desk-clock configuration.

## ⚙️ Tools Used
* **EDA Tool:** KiCad (Schematic Capture, PCB Layout, and 3D Visualizer Integration)

## 📺 Demo Video
Click the image below to watch the hardware platform and interface in action:

[![Watch the video](https://shields.io)](https://1drv.ms/v/c/b2abd14c679eea6b/IQBb18cBuQbQQaUBIMpuPMWnAfBBgvG3fzTZn4pLQCEiL4w?e=841tbs)

*[Click here to watch the full project demonstration if the badge above doesn't open.](https://1drv.ms/v/c/b2abd14c679eea6b/IQBb18cBuQbQQaUBIMpuPMWnAfBBgvG3fzTZn4pLQCEiL4w?e=841tbs)*
