# 🧵 PLA Print Settings

Part of the [Purpose in Practice 3D Printing Workshop](../README.md).

PLA is one of the most accessible materials in 3D printing.

Although I primarily use PETG for functional projects, PLA is a useful option for prototypes, decorative objects, and parts that don't require additional heat resistance.

This page covers recommended PLA starting settings for the **Bambu Lab A1**, along with practical printing tips and troubleshooting.

---

## 🖨️ My Equipment

| Equipment | Product |
|---|---|
| Printer | [Bambu Lab A1](https://geni.us/2uwo9G) |
| Build Plate | [BIQU CryoGrip Pro Glacier](https://geni.us/ubKy1) |
| Slicer | Bambu Studio |
| Nozzle | 0.4 mm (standard configuration) |

**Note:** PLA is not my primary printing material. The settings below are general starting recommendations, not a record of my personally tested PLA profiles.

---

## ⚙️ PLA Starting Settings

The easiest starting point is the appropriate PLA filament profile in Bambu Studio.

For standard PLA, the following settings provide a reasonable reference.

| Setting | Starting Point |
|---|---|
| Nozzle temperature | 190–220°C |
| Bed temperature | Follow build plate and filament recommendations |
| Layer height | 0.20 mm |
| First layer height | 0.20 mm |
| Wall loops | 2–3 |
| Top shell layers | 4–5 |
| Bottom shell layers | 4–5 |
| Infill | 10–20% |
| Infill pattern | Gyroid or adaptive cubic |
| Cooling | Use the selected PLA profile |
| Print speed | Start with Bambu Studio defaults |
| Retraction | Use the printer's default profile |

These values may need adjustment depending on the filament brand, nozzle size, print geometry, and intended application.

High-speed PLA formulations may use different temperature and flow settings.

---

## 🔥 Nozzle Temperature

PLA generally prints at lower temperatures than PETG.

If the nozzle temperature is too low, you may experience:

- Poor layer adhesion
- Under-extrusion
- Rough surfaces
- Weak prints

If the nozzle temperature is too high, you may experience:

- Stringing
- Blobs
- Excessive oozing
- Poor overhangs

Start with the filament manufacturer's recommended profile before making adjustments.

---

## 🔲 Build Plate & Adhesion

My primary build plate is the **BIQU CryoGrip Pro Glacier**.

**[BIQU CryoGrip Pro Glacier — Compare Prices](https://geni.us/ubKy1)**

The Glacier is designed to provide strong adhesion at relatively low bed temperatures for compatible materials.

### Tips

- Keep the plate clean.
- Avoid touching the printing surface.
- Verify that the selected Bambu Studio build plate configuration is appropriate.
- Follow BIQU's temperature and cleaning recommendations.
- Allow the plate to cool before removing prints.
- Avoid scraping aggressively or using tools that could damage the coating.

**Important:** Specialty build plates may require different temperatures from standard textured PEI plates. Don't automatically apply generic PLA bed temperatures to the CryoGrip Glacier.

---

## 🌬️ Cooling

PLA generally benefits from effective part cooling.

Good cooling helps with:

- Overhangs
- Bridges
- Small details
- Surface finish
- Dimensional accuracy

However, excessive cooling can sometimes reduce layer adhesion or cause problems with certain geometries.

The default Bambu Studio PLA profile is a good starting point.

---

## 🧱 Walls, Infill & Strength

For many PLA prints, two or three wall loops and moderate infill are sufficient.

### Prototypes

For basic test prints:

- 2 wall loops
- 10–15% infill
- 0.20 mm layer height

These settings can help reduce printing time and material usage.

### Functional Parts

For parts that need additional strength:

- Consider 3 or more wall loops.
- Adjust infill based on the application.
- Pay attention to print orientation.
- Avoid relying on PLA for applications that experience significant heat or sustained mechanical stress.

Adding more walls can sometimes improve strength more effectively than increasing infill.

---

## 🌡️ Heat Resistance

One limitation of PLA is its relatively low heat resistance.

PLA can begin to soften or deform at temperatures that may occur inside hot vehicles, near heating equipment, or in direct sunlight.

For electronics enclosures and other functional projects, I generally prefer PETG when additional heat resistance is useful.

See [PETG Print Settings](PETG.md).

---

## 💧 Filament Storage

PLA can also absorb moisture.

Wet filament may contribute to:

- Stringing
- Popping during extrusion
- Rough surfaces
- Inconsistent extrusion
- Reduced print quality

Store filament in a dry environment and follow the manufacturer's drying recommendations when necessary.

---

## 🛠️ Troubleshooting

| Problem | Possible Cause | What to Try |
|---|---|---|
| Stringing | Moisture or excessive temperature | Dry filament; review temperature |
| Poor bed adhesion | Dirty plate or incorrect settings | Clean plate; verify temperature |
| Warping | Poor adhesion or uneven cooling | Check first layer and plate settings |
| Weak layers | Low temperature or excessive cooling | Review temperature and cooling |
| Rough surfaces | Moisture or flow problems | Check filament condition and profile |
| Poor overhangs | Insufficient cooling | Review fan settings |
| Elephant's foot | Excessive first-layer squish or heat | Check first layer and compensation |
| Dimensional problems | Flow or tolerance issues | Print a calibration part |

For additional guidance, see [Troubleshooting](Troubleshooting.md).

---

## 🧪 Testing Notes

As I experiment with PLA, I'll document actual results here.

| Test | Result |
|---|---|
| First-layer adhesion | To be documented |
| Dimensional accuracy | To be documented |
| Bridging and overhangs | To be documented |
| Surface finish | To be documented |
| Strength | To be documented |

These notes will be updated with actual print results.

---

## 💡 When I'd Choose PLA Instead of PETG

PLA makes sense when:

- I'm creating a quick prototype.
- The part is primarily decorative.
- I want fine detail and a clean surface finish.
- Heat resistance isn't a major concern.
- The part won't experience significant mechanical stress.

PETG remains my preferred material for many electronics enclosures, brackets, and household applications.

---

## Affiliate Disclosure

Some product links on this page are affiliate links. I may earn a commission from qualifying purchases at no additional cost to you. These links help support future Purpose in Practice projects.

---

*Learn it. Build it. Put it into practice.*

**Purpose in Practice**
