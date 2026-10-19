# 🔐 ESPHome Alarmo Keypad — 3D-Printed Enclosure

Part of the [Purpose in Practice 3D Printing Workshop](../../README.md).

Sometimes a project works perfectly well electrically but looks like something you assembled from spare parts in the garage.

That's pretty much how my ESPHome Alarmo Keypad started.

The original prototype used an ESP32-C3, physical keypad, OLED display, and buzzer stuffed into a basic project box.

It worked.

But I wanted something that looked a little more finished and could be mounted on the wall.

That's where 3D printing came in.

---

## 🏠 About the Project

The ESPHome Alarmo Keypad is a dedicated physical control panel for **Home Assistant and Alarmo**.

Instead of relying entirely on a touchscreen or phone, it provides a physical keypad for interacting with the alarm system.

The hardware includes:

- ESP32-C3 Super Mini
- 4×4 matrix keypad
- SSD1306 OLED display
- Audible buzzer
- Custom PCB
- 3D-printed enclosure

The enclosure brings those components together into a cleaner, wall-mounted design.

---

## 🖨️ The 3D-Printed Enclosure

The goal was to create an enclosure that:

- Holds the keypad securely
- Provides an opening for the OLED display
- Accommodates the custom PCB
- Allows access to the required connections
- Provides a practical way to mount the device
- Looks more finished than the original prototype

The design evolved alongside the electronics.

Moving from loose wiring to a custom PCB made it possible to build a more organized enclosure around the actual hardware.

---

## ⚙️ My Printing Equipment

| Equipment | Product |
|---|---|
| Printer | [Bambu Lab A1](https://geni.us/2uwo9G) |
| Primary Filament | [Bambu PETG Basic](https://geni.us/4HC3cQ) |
| Additional Filament | [Bambu PETG Translucent](https://geni.us/jEhyD) |
| Build Plate | [BIQU CryoGrip Pro Glacier](https://geni.us/ubKy1) |
| Slicer | Bambu Studio |

These are the products I currently use in my workshop. The exact filament and settings used for individual enclosure revisions will be documented as they're confirmed.

For general printing guidance, see [PETG Print Settings](../../Print-Settings/PETG.md).

---

## 📂 Download the Printable Files

The printable enclosure files are maintained in the main Alarmo Keypad repository.

**[View the Alarmo Keypad 3D Print Files](https://github.com/loperkin/another-esphome-alarmo-keypad/tree/main/3D%20Print)**

The repository also includes the ESPHome configuration, electronics information, and PCB files.

**[Complete ESPHome Alarmo Keypad Project](https://github.com/loperkin/another-esphome-alarmo-keypad)**

This workshop page is intended to provide additional 3D-printing information without creating multiple copies of the same design files.

---

## 🔧 Hardware & Components

If you're building the complete keypad, these are the main components used in the project.

| Component | Product Link |
|---|---|
| ESP32-C3 Super Mini | [Compare Prices](https://geni.us/mZse) |
| 4×4 Matrix Keypad | [Compare Prices](https://geni.us/rCXY0aQ) |
| SSD1306 OLED Display | [Compare Prices](https://geni.us/LMIEOmU) |
| Active Buzzer — Original Version | [Compare Prices](https://geni.us/1eZhR) |
| Passive Buzzer — PCB Version | [Compare Prices](https://geni.us/zDvK1YI) |

Check the main project documentation before purchasing components, as the prototype and custom PCB versions have different hardware requirements.

---

## 🛒 Finished Hardware & Parts

For anyone who wants to use the keypad without manufacturing every component themselves, I also offer hardware options.

- **[Complete Keypad Hardware](https://py.pl/1fJqHh)** — Assembled electronics with a 3D-printed enclosure
- **[Bare Custom PCB](https://py.pl/1d8C3f)** — PCB for building your own
- **[3D-Printed Enclosure](https://py.pl/7ZUzHRGNsK6)** — Printed case only

Availability and pricing may change.

---

## 🧪 Design Notes & Lessons Learned

One of the biggest improvements was moving away from the original project box and designing an enclosure around a custom PCB.

That made it easier to organize the components and create a cleaner finished assembly.

This project also reinforced a few useful lessons:

1. Design around the actual dimensions of the hardware.
2. Account for PCB mounting holes and component clearances.
3. Leave enough room for wiring and connectors.
4. Think about assembly before finalizing the enclosure.
5. Expect the first design to need adjustments.

A printed enclosure can make a prototype feel like a finished product, but only if everything actually fits.

---

## 🔄 Future Updates

As I revise the enclosure, I'll document:

- Changes to the printed design
- Assembly improvements
- Updated print settings
- Material choices
- Mounting improvements
- Lessons learned from additional builds

The current printable files will remain in the main Alarmo Keypad repository.

---

## 📜 Licensing & Attribution

Original printable designs are covered by the licensing terms in the main project repository.

Review the [Alarmo Keypad repository](https://github.com/loperkin/another-esphome-alarmo-keypad) before modifying or redistributing its files.

For general licensing information about
