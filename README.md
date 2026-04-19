# SL-814 dB Meter

A web-based interface for the **Tondaj SL-814 sound level meter**. Connects via USB-to-serial adapter and displays real-time decibel readings with a smooth animated VU meter visualization. Runs in Chrome or Edge only (uses Web Serial API).

<img width="1316" height="668" alt="Screenshot 2026-02-07 230753" src="https://github.com/user-attachments/assets/db4303e2-5ee6-4750-aa80-1cf810395869" />

## Features

- Real-time dB readings with 60fps animated bar
- Peak hold indicator
- A/C weighting and Fast/Slow mode display
- Light/Dark theme
- English/Slovak language support
- No installation required — runs directly in browser

## How to Run

1. Connect the SL-814 meter to your PC via USB-to-serial cable (Prolific PL2303)
2. Open `SL-814 dB meter.html` in **Chrome** or **Edge**
3. Click "Choose device & start" and select the COM port
4. Readings will stream automatically

> **Note:** The Web Serial API requires Chrome or Edge. Firefox and Safari are not supported.

## Driver Installation (Windows 11)

The Prolific PL2303 adapter requires legacy drivers on Windows 11. See [driver/README.md](driver/README.md) for detailed instructions.

**Quick steps:**
1. Download drivers from [theAmberLion/Prolific](https://github.com/theAmberLion/Prolific) or from this repo "[SL-814-dB-meter/driver](https://github.com/DotaPie/SL-814-dB-meter/tree/main/driver)"
2. Install `PL2303_Prolific_v3.3.2.105.exe`
3. In Device Manager, update the driver and select version 3.3.2.105

## Protocol Reference

Serial protocol reverse-engineered by the sigrok project:  
https://sigrok.org/wiki/Tondaj_SL-814
