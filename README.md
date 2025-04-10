# 🔧 Custom ESP32 Dev Board – WROOM + CH340

This project is a custom ESP32 development board designed from scratch, featuring the **ESP32-WROOM-32** module and **CH340** USB-to-serial converter. Built for embedded projects and prototyping, this board brings together reliability, compact design, and ease of programming.



## 📁 Files Included
- `.fbrd` – Fusion 360 PCB board file  
- `.fsh` – Fusion 360 schematic file

> 💡 *Designed entirely in Fusion 360 Electronics.*

## ⚙️ Features
- **ESP32-WROOM-32** module with WiFi + Bluetooth
- **CH340** USB to UART converter for easy flashing
- USB-C or Micro-USB input (depending on version)
- 3.3V LDO regulator
- Onboard reset and boot buttons
- All essential I/O pins broken out
- Compact 2-layer PCB design

## 🛠️ Tools Used
- **Fusion 360 Electronics** for schematic + PCB layout  
- **PlatformIO + VS Code** for firmware development  
- **Cura + 3D printer** for potential enclosure prototyping

## 💻 Flashing & Development

This board is compatible with PlatformIO. You can use the Freenove ESP32-WROOM environment for development. Just copy this `platformio.ini` into your project:

```ini
[env:esp32dev]
platform = espressif32
board = freenove_esp32_wrover
framework = arduino
upload_speed = 115200
monitor_speed = 115200
