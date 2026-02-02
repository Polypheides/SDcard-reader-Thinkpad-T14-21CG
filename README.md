# ⚠️ Disclaimer: This PCB is UNTESTED ⚠️

**Use at your own risk.** This is an experimental project and has not yet been verified in physical hardware.

## Project Overview

This project provides **Gerber** files for an internal SD card reader daughterboard designed for the **ThinkPad T14 (Gen 3/21CG)**. It is designed to replace the original right-side single USB daughterboard.

### Key Technical Specs (Rev. 5)

* **Controller:** GL823K USB 2.0 SD Card Reader.


* **USBLC6-2SC6** monolithic ESD protection device.

* **High-Speed Data Integrity:** Features a very low capacitance of $1\text{ pF}$, ensuring that the USB 2.0 differential signals ($D+/D-$) remain crisp and within specification.

* **Comprehensive Protection:** Provides ESD protection for Data- Clock- and Command-signals.

* **Rail-to-Rail Protection:** Effectively clamps high-voltage spikes from static electricity before they reach the **GL823K** controller or the ThinkPad's internal Hub.



* **Interface:** Custom 20-pin FPC/Board-to-board connector (CON1).


* **Manufacturing Note:** Recommended PCB thickness is **1.0 mm** for correct chassis fitment.

### Installation Notes

* **Chassis Modding:** Physical filing of the laptop's plastic/magnesium frame may be required as the SD slot is wider than the original USB-A opening.
* **Orientation:** Pin 1 on the PCB must match Pin 1 on the motherboard connector.
