# 🏠 ESPHome MultiSensor — 3D-Printed Enclosures

Part of the [Purpose in Practice 3D Printing Workshop](../../README.md).

One of the reasons I got into 3D printing was to make my electronics projects look less like experiments and more like something that actually belongs in the house.

My ESPHome MultiSensor projects are a good example.

What started as a collection of sensors and an ESP32 eventually evolved into custom PCBs and 3D-printed enclosures.

And like most of my projects, the first version wasn't the last.

---

## 🔍 About the MultiSensor

The ESPHome MultiSensor combines several sensors into one device:

- **mmWave presence detection** using the LD2410C
- **Ambient light sensing** using the BH1750
- **Temperature and humidity** using the DHT22
- **ESP32-C3 Super Mini** microcontroller
- **ESPHome** firmware
- **Home Assistant** integration

The goal is to provide useful room-level information for home automation.

For example, presence detection can help control lighting, while temperature readings can be used in room-based HVAC automations.

---

## 🖨️ Original MultiSensor Enclosure

The original MultiSensor began as a prototype using individual modules and wiring.

As the project developed, I created a custom PCB to make the electronics easier to assemble and more compact.

A 3D-printed enclosure helps protect the components and provides a cleaner way to install the device.

### Design Goals

- Hold the electronics securely
- Provide appropriate openings for sensors
- Allow power connections
- Support practical installation
- Make assembly and maintenance easier
- Keep the design reasonably compact

### Project Repository

**[ESPHome MultiSensor — Presence, Light, Temperature & Humidity](https://github.com/loperkin/ESPHome-MultiSensor-presence-light-temp-hum)**

The main repository contains the project's electronics, ESPHome configuration, documentation, and available design resources.

---

## 🔌 MultiSensor Decora Enclosure

The next evolution of the project is the **ESPHome MultiSensor Decora**.

Instead of mounting a separate sensor box on the wall, I wanted to integrate the electronics into a Decora-style wall plate.

The idea was to create something that looks more like a permanent part of the house.

### Design Goals

- Fit a Decora-style wall installation
- Integrate a custom PCB
- Accommodate the presence, light, temperature, and humidity sensors
- Provide a cleaner appearance
- Allow maintenance and future hardware revisions
- Reduce the visual clutter of separate sensor devices

### The Challenge: Temperature Accuracy

One issue I've been working through is temperature measurement.

Putting electronics into a compact enclosure can introduce heat-related measurement errors.

The ESP32, power supply, surrounding electronics, and enclosure design can influence the temperature reported by the sensor.

A sensor that consistently reads warmer than the room isn't particularly useful for controlling HVAC equipment.

This is one of the reasons enclosure design matters beyond appearance.

I'm continuing to refine the design and evaluate ways to improve temperature accuracy.

### Project Repository

**[ESPHome MultiSensor Decora](https://github.com/loperkin/ESPHome-MultiSensor-Decora)**

The Decora repository is the home for that version's firmware, PCB design, printable components, and related documentation.

**Development note:** The Decora design is an evolving project. Check its repository for the current revision and known limitations before building it.

---

## 🖨️ My 3D Printing Equipment

| Equipment | Product |
|---|---|
| Printer | [Bambu Lab A1](https://geni.us/2uwo9G) |
| Primary Filament | [Bambu PETG Basic](https://geni.us/4HC3cQ) |
| Additional Filament | [Bambu PETG Translucent](https://geni.us/jEhyD) |
| Build Plate | [BIQU CryoGrip Pro Glacier](https://geni.us/ubKy1) |
| Slicer | Bambu Studio |

These are the products currently used in my workshop. The exact material and settings for each enclosure revision will be documented as they're confirmed.

See [PETG Print Settings](../../Print-Settings/PETG.md) for general printing guidance.

---

## 🔧 Electronics & Components

These are the primary components used in the MultiSensor projects.

| Component | Product Link |
|---|---|
| ESP32-C3 Super Mini | [Compare Prices](https://geni.us/mZse) |
| LD2410C mmWave Sensor | [Compare Prices](https://geni.us/TfpZvN) |
| BH1750 Light Sensor | [Compare Prices](https://geni.us/sySYq0f) |
| DHT22 Temperature/Humidity Sensor | [Compare Prices](https://geni.us/jqC5I) |

The original and Decora versions have different physical layouts and hardware requirements.

Review the appropriate project repository before ordering parts.

---

## 🧪 Design Considerations

### Sensor Placement

Sensor placement is important.

An enclosure must allow the sensors to operate without introducing unnecessary interference.

For example:

- Temperature sensors need exposure to representative room air.
- Light sensors need appropriate exposure to ambient light.
- mmWave sensors require suitable placement and compatible enclosure materials.
- Electronics need adequate clearance and ventilation.

### Heat Management

Heat from electronic components can affect temperature measurements.

Possible improvements include:

- Increasing separation between heat-producing components and temperature sensors
- Improving airflow around the sensor
- Reducing thermal conduction through the PCB
- Evaluating alternative sensor placement
- Testing readings against an independent room thermometer

These are design considerations rather than confirmed fixes for the Decora version.

### Assembly & Maintenance

A good enclosure should also make the electronics accessible.

I try to consider:

- PCB mounting
- Wire routing
- Component clearances
- Fasteners
- Access for troubleshooting
- Ease of replacing components

A beautiful enclosure isn't much use if you have to destroy it to fix a loose connection.

---

## 📂 Printable Files & Documentation

Rather than maintain duplicate design files in multiple repositories, the individual MultiSensor repositories remain the primary sources for their respective designs.

### Original MultiSensor

[View the Original MultiSensor Repository](https://github.com/loperkin/ESPHome-MultiSensor-presence-light-temp-hum)

### MultiSensor Decora

[View the MultiSensor Decora Repository](https://github.com/loperkin/ESPHome-MultiSensor-Decora)

Check the repositories for current files, revisions, assembly information, and project-specific licensing.

---

## 🔄 Future Updates

As these projects evolve, I'll document:

- New enclosure revisions
- Changes to PCB mounting
- Material selection
- Print settings
- Sensor placement improvements
- Temperature measurement testing
- Assembly improvements
- Lessons learned from installation

The goal is to create something that's not only functional but also practical to reproduce.

---

## 💡 Lessons Learned

Building an enclosure for electronics is different from printing a decorative object.

The enclosure becomes part of the system.

Its shape, material, ventilation, and component placement can affect how the electronics perform.

Sometimes the hardest part isn't getting everything to fit.

It's getting everything to work correctly once it does.

---

## 📜 Licensing & Attribution

Review the licensing terms in each project's main repository before modifying, redistributing, or manufacturing its designs.

For general workshop licensing information, see [LICENSE.md](../../LICENSE.md).

---

## Affiliate Disclosure

Some product links on this page are affiliate links. I may earn a commission from qualifying purchases at no additional cost to you. These links help support future Purpose in Practice projects.

---

*Learn it. Build it. Put it into practice.*

**Purpose in Practice**
