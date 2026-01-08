# Control Your Gree Air Conditioner with Touch GX

### Using Victron Venus OS & Node-RED

Control a **Gree split system air conditioner** directly from a **Victron Touch GX** using **Venus OS** and **Node-RED**.
This project allows seamless integration of household or caravan air conditioning into the Victron ecosystem for monitoring, automation, and remote control.

Ideal for **off-grid homes, caravans, RVs, and marine installations** where Victron equipment is already in use.

---

## Features

* Control Gree air conditioners from the **Touch GX screen**
* Power, mode, fan speed, and temperature control
* Node-RED dashboard integration
* Automation support (battery SOC, inverter load, schedules, temperature)
* Works locally (no cloud dependency)
* Designed for Venus OS Large

---

## System Overview

The system works by:

* Running **Node-RED** on Venus OS
* Communicating with the **Gree AC local API**
* Exposing controls and status to the **Victron GUI**
* Allowing automation logic based on Victron data (battery, solar, inverter state)

---

## Requirements

### Hardware

* Victron GX device (Cerbo GX, Raspberry Pi with Venus OS, etc.)
* Victron Touch GX (50 or 70)
* Gree air conditioner with Wi-Fi module
* Local network (GX device and AC on same LAN)

### Software

* Venus OS (Large image recommended)
* Node-RED enabled
* Gree AC configured and accessible on local network

---

## Supported Air Conditioners

* Gree Wi-Fi enabled split systems
* Models using the standard Gree local LAN protocol

Other brands that re-use the Gree protocol may also work but are untested.

---

## Installation Summary

1. Install **Venus OS Large**
2. Enable **Node-RED**
3. Import the provided Node-RED flow
4. Configure:

   * Gree AC IP address
   * Device ID / key (if required)
5. Access the Node-RED dashboard from the Touch GX

---

## Automation Examples

* Disable AC when battery SOC drops below a set level
* Only allow AC operation when solar production is sufficient
* Pre-cool or pre-heat before arriving home
* Schedule operation by time or temperature

---

## Touch GX Integration

* Uses Node-RED Dashboard
* Optimised for Touch GX screen size
* Can be launched directly from the Venus OS GUI

---

## Limitations

* Local network required
* No official Gree API support (reverse-engineered protocol)
* Firmware updates to the AC may affect compatibility

---

## Disclaimer

This project is **not affiliated with or endorsed by Gree or Victron Energy**.
Use at your own risk. Always ensure electrical and HVAC work complies with local regulations.

---

## Contributing

Pull requests, improvements, and testing feedback are welcome.

---

## License

MIT License

---

## Screenshots

*Add screenshots of the Touch GX interface here*

---

## Credits

* Victron Energy – Venus OS & GX platform
* Node-RED community
* Gree protocol reverse-engineering contributors

