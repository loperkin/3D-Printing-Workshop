# 🧵 PETG Print Settings

Part of the [Purpose in Practice 3D Printing Workshop](../README.md).

PETG is my primary 3D printing material.

I use it for electronics enclosures, brackets, mounting hardware, prototypes, and other functional parts that need a little more toughness and heat resistance than standard PLA.

My printer is a **Bambu Lab A1**, and I primarily use **Bambu Lab PETG Basic** and **Bambu Lab PETG Translucent**.

This page documents my printing setup, recommended starting points, troubleshooting tips, and lessons learned.

---

## 🖨️ My Equipment

| Equipment | Product |
|---|---|
| Printer | [Bambu Lab A1](https://geni.us/2uwo9G) |
| Primary Filament | [Bambu PETG Basic](https://geni.us/4HC3cQ) |
| Additional Filament | [Bambu PETG Translucent](https://geni.us/jEhyD) |
| Build Plate | [BIQU CryoGrip Pro Glacier](https://geni.us/ubKy1) |
| Slicer | Bambu Studio |

The settings discussed here assume a standard 0.4 mm nozzle. Other nozzle sizes may require different settings.

---

## ⚙️ PETG Starting Settings

These are general starting points for PETG on the Bambu Lab A1.

**Start with the appropriate Bambu Studio filament profile**, then make adjustments based on the specific filament and the results of test prints.

| Setting | Starting Point |
|---|---|
| Nozzle temperature | 230–255°C |
| Bed temperature | Follow filament and build plate recommendations |
| Layer height | 0.20 mm |
| First layer height | 0.20 mm |
| Wall loops | 3 |
| Top shell layers | 4–5 |
| Bottom shell layers | 4–5 |
| Infill | 15–25% |
| Infill pattern | Gyroid or adaptive cubic |
| Cooling | Moderate; use the filament profile |
| Print speed | Start with the Bambu Studio PETG profile |
| Retraction | Start with the printer's default profile |

These values are starting recommendations, not a universal profile.

For functional parts, geometry, wall thickness, print orientation, and layer adhesion can matter more than simply increasing infill.

---

## 🔥 Nozzle Temperature

PETG generally requires higher extrusion temperatures than PLA.

If the nozzle temperature is too low, you may experience:

- Poor layer adhesion
- Under-extrusion
- Weak parts
- Rough surfaces

If the temperature is too high, you may experience:

- Increased stringing
- Blobs
- Excessive oozing
- Surface defects

The best temperature depends on the specific filament, print speed, and cooling configuration.

I recommend beginning with the manufacturer's filament profile rather than immediately changing temperatures.

---

## 🔲 Build Plate & Adhesion

My primary build plate is the **BIQU CryoGrip Pro Glacier**.

[BIQU CryoGrip Pro Glacier — Compare Prices](https://geni.us/ubKy1)

Reliable first-layer adhesion is important, especially for taller prints or projects with relatively small contact areas.

### Tips

- Keep the build plate clean.
- Avoid touching the printing surface unnecessarily.
- Use a compatible build plate selection in Bambu Studio.
- Follow BIQU's temperature and maintenance recommendations for the Glacier coating.
- Let prints cool before removing them.
- Avoid forcing prints off the surface with sharp tools.

**Important:** Do not assume that a generic PETG bed temperature is appropriate for a specialty low-temperature build plate. Verify the recommended temperature for the specific plate and material.

---

## 🧱 Walls, Infill & Strength

Most of my projects involve functional parts.

For electronics enclosures, brackets, and mounting hardware, I generally prioritize durability and dimensional accuracy.

### Wall Loops

Three wall loops are a reasonable starting point for many functional parts.

Additional walls can improve strength, depending on the geometry and direction of the forces involved.

### Infill

For many functional prints, 15–25% infill provides a useful starting range.

Increasing infill doesn't always produce the best improvement in strength.

Sometimes adding walls or changing print orientation makes a bigger difference.

### Print Orientation

Layer orientation is especially important for brackets, clips, and other parts that experience mechanical stress.

A part may be strong in one direction and much weaker in another.

I try to orient prints so that the expected forces are less likely to separate the layers.

---

## 🌡️ Cooling

Cooling affects surface finish, overhang quality, and layer bonding.

Too much cooling can reduce layer adhesion.

Too little cooling can cause poor bridges, sagging overhangs, and other defects.

For PETG, I recommend starting with the cooling settings included in the selected Bambu Studio filament profile.

Small parts and complex overhangs may require additional tuning.

---

## 💧 Moisture & Filament Drying

PETG can absorb moisture from the surrounding air.

Moisture can contribute to:

- Stringing
- Popping or crackling during extrusion
- Rough surfaces
- Inconsistent extrusion
- Reduced mechanical performance

If print quality deteriorates unexpectedly, moisture is one possible cause worth investigating.

Dry filament according to the manufacturer's recommendations, and store it in a dry environment.

Drying temperature and duration should be appropriate for both the filament and the equipment being used.

---

## 🔍 PETG Basic vs. PETG Translucent

I use two main PETG materials.

### Bambu Lab PETG Basic

[PETG Basic — Compare Prices](https://geni.us/4HC3cQ)

My primary choice for:

- Electronics enclosures
- Brackets and mounts
- Functional household parts
- Prototypes
- General-purpose printing

### Bambu Lab PETG Translucent

[PETG Translucent — Compare Prices](https://geni.us/jEhyD)

Useful for:

- Light diffusers
- LED indicators
- Electronics cases with internal lighting
- Parts where translucency improves the design

The appearance of translucent PETG depends on wall thickness, infill, print orientation, and surface finish.

It may also require different settings from PETG Basic.

I treat them as separate filament profiles rather than assuming identical behavior.

---

## 🛠️ Troubleshooting

| Problem | Possible Cause | What to Try |
|---|---|---|
| Stringing | Moisture, temperature, travel behavior | Dry filament; review temperature and retraction |
| Poor bed adhesion | Dirty plate, incorrect plate settings | Clean plate; verify settings |
| Weak layer bonding | Low temperature, excessive cooling | Review temperature and cooling |
| Blobs or zits | Moisture, oozing, flow settings | Dry filament; check profile |
| Rough surfaces | Moisture, temperature, speed | Check filament condition and profile |
| Warping | Uneven cooling, poor adhesion | Review first layer and cooling |
| Poor overhangs | Insufficient cooling or excessive heat | Adjust cooling and print orientation |
| Poor dimensional fit | Tolerances, flow, model design | Print a test piece and adjust clearances |

For more detailed troubleshooting, see [Troubleshooting](Troubleshooting.md).

---

## 🧪 My Testing Notes

As I refine my PETG profiles, I'll document actual results here.

| Test | Setting / Material | Result |
|---|---|---|
| First-layer adhesion | PETG Basic + CryoGrip Glacier | To be documented |
| Dimensional accuracy | PETG Basic | To be documented |
| Stringing | PETG Basic | To be documented |
| Translucency | PETG Translucent | To be documented |
| Strength | Functional PETG parts | To be documented |

I'll update this table with actual measurements and observations rather than guessing.

---

## 💡 Lessons Learned

A few principles I keep in mind:

1. Start with a known-good filament profile.
2. Change one setting at a time when troubleshooting.
3. Dry filament when moisture may be affecting quality.
4. Design parts around their intended use.
5. Print small test pieces before committing to a long print.
6. Don't assume that more infill automatically means a stronger part.

The goal isn't necessarily to produce the fastest print.

It's to produce a part that works.

---

## Affiliate Disclosure

Some product links on this page are affiliate links. I may earn a commission from qualifying purchases at no additional cost to you. These links help support future Purpose in Practice projects.

---

*Learn it. Build it. Put it into practice.*

**Purpose in Practice**
