# ⚠️ Disclaimer: Rev. 7 PCB Tested with Known Issues ⚠️

**Use at your own risk.** This is an experimental project. Rev. 7 has been hardware-verified to work, but requires a bodge wire fix.

> [!IMPORTANT]
> <details>
>   <summary><b>View Rev. 7 Bodge Wire Photo</b></summary>
>   <br>
>   <img src="Misc/Images/Rev.%207%20Botch%20Wire.jpg" alt="Rev. 7 Botch Wire" width="450">
> </details>

---

## Project Overview

This repository provides **Gerber files** for an internal MicroSD card reader daughterboard designed for the **ThinkPad T14 (Gen 3 / 21CG)**. It replaces the stock right-side single USB daughterboard.

### Technical Specifications

* **Controller:** Genesys Logic **GL823K** (USB 2.0 MicroSD Card Reader Controller).
* **ESD Protection:** **USBLC6-2SC6** monolithic ESD protection array.
  * **Data Integrity:** Ultra-low line capacitance (1 pF) prevents signal degradation on USB 2.0 differential pairs (D+/D-).
  * **Line Coverage:** Dedicated ESD clamping for data, clock, and command lines.
  * **Rail-to-Rail Clamping:** Suppresses high-voltage electrostatic discharge before transients reach the controller or internal hub.
* **Interface:** 20-pin FPC / board-to-board connector (`CON1`).
* **PCB Thickness:** Recommended **1.0 mm** for proper chassis clearance and alignment.

> [!NOTE]
> Rev.8 integrates the missing trace fix from Rev. 7 (eliminating the need for a jumper wire) and adds additional decoupling capacitors for power rail stability.

---

## Installation & Fitment Notes

* **Chassis Modification:** Physical filing or trimming of the laptop's plastic/magnesium subframe should not be required.
* **Connector Orientation:** Ensure **Pin 1** on the daughterboard aligns with **Pin 1** on the motherboard connector before applying power.
