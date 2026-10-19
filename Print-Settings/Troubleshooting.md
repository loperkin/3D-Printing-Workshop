# 🔧 3D Printing Troubleshooting

Part of the [Purpose in Practice 3D Printing Workshop](../README.md).

Sometimes a print comes out exactly as planned.

Other times, you come back to find a pile of plastic spaghetti where your project was supposed to be.

This page is a troubleshooting reference for common 3D printing problems, what might cause them, and how to fix them.

My primary setup is a **Bambu Lab A1** using **Bambu Lab PETG** and a **BIQU CryoGrip Pro Glacier** build plate.

The goal is to document useful troubleshooting methods and, over time, add solutions from my own projects.

---

## 🖨️ My Printing Setup

| Equipment | Product |
|---|---|
| Printer | [Bambu Lab A1](https://geni.us/2uwo9G) |
| Primary Filament | [Bambu PETG Basic](https://geni.us/4HC3cQ) |
| Additional Filament | [Bambu PETG Translucent](https://geni.us/jEhyD) |
| Build Plate | [BIQU CryoGrip Pro Glacier](https://geni.us/ubKy1) |
| Slicer | Bambu Studio |

Related guides:

- [PETG Print Settings](PETG.md)
- [PLA Print Settings](PLA.md)
- [Build Plates](../Equipment/Build-Plates.md)
- [Filament & Materials](../Equipment/Filament.md)

---

## 🔍 Quick Troubleshooting Reference

| Problem | Possible Causes | First Things to Try |
|---|---|---|
| Print won't stick | Dirty plate, incorrect plate settings, first-layer issue | Clean plate and verify settings |
| Stringing | Wet filament, temperature, retraction | Dry filament and check profile |
| Warping | Poor adhesion, cooling, part geometry | Review plate settings and add a brim |
| Layer separation | Low temperature, excessive cooling | Check temperature and fan settings |
| Blobs or zits | Moisture, oozing, flow inconsistencies | Dry filament and inspect profile |
| Rough surfaces | Moisture, extrusion problems, excessive speed | Check filament and flow settings |
| Elephant's foot | Excessive first-layer compression or heat | Review first-layer settings |
| Poor overhangs | Insufficient cooling, speed, orientation | Review cooling and supports |
| Inaccurate dimensions | Model tolerances, flow, shrinkage | Measure a test print |
| No extrusion | Clog, filament feed issue, temperature | Check filament path and nozzle |
| Spaghetti failure | Loss of adhesion, detached support, collision | Inspect first layer and supports |
| Layer shifting | Mechanical interference, collision, belt issue | Check for obstructions and mechanical problems |

---

## 🔲 1. Poor Bed Adhesion

### Symptoms

- First layer doesn't stick.
- Corners lift from the plate.
- Small parts detach during printing.
- The nozzle drags loose filament around the bed.

### Possible Causes

- Dirty build plate
- Incorrect plate temperature
- Incompatible build plate profile
- First-layer extrusion problems
- Insufficient contact area
- Wet or contaminated filament

### What to Try

1. Clean the build plate according to its manufacturer's instructions.
2. Verify the selected build plate in Bambu Studio.
3. Confirm the bed temperature is appropriate for the filament and plate.
4. Inspect the first layer for consistent extrusion.
5. Add a brim when printing parts with limited bed contact.
6. Run the printer's calibration procedures when appropriate.

### My Build Plate

I use the **BIQU CryoGrip Pro Glacier**.

**[BIQU CryoGrip Pro Glacier — Compare Prices](https://geni.us/ubKy1)**

This plate has helped improve adhesion in my workshop.

**Important:** Specialty build plates may require different temperatures and cleaning procedures from standard PEI plates. Follow the instructions for the actual surface you're using.

---

## 🕸️ 2. Stringing

### Symptoms

Thin strands of filament appear between separate sections of a print.

### Possible Causes

- Moisture in the filament
- Excessive nozzle temperature
- Oozing during travel moves
- Retraction or travel settings
- Filament-specific behavior

### What to Try

1. Check whether the filament needs drying.
2. Start with the correct Bambu Studio filament profile.
3. Test a slightly lower nozzle temperature within the manufacturer's recommended range.
4. Review travel and retraction settings.
5. Change one variable at a time.

PETG is generally more prone to stringing than PLA.

Don't assume retraction is the problem before checking filament moisture.

---

## 📐 3. Warping & Lifting Corners

### Symptoms

- Corners curl upward.
- The bottom of a print becomes uneven.
- The print separates from the bed.

### Possible Causes

- Poor bed adhesion
- Uneven cooling
- Large flat surfaces
- Part geometry
- Incorrect bed temperature

### What to Try

- Clean the build plate.
- Verify the bed temperature.
- Add a brim.
- Review cooling settings.
- Reorient the model when practical.
- Consider modifying the design to reduce stress concentrations.

A brim can be particularly helpful for tall, narrow parts or models with small contact areas.

---

## 🧱 4. Weak Layers & Layer Separation

### Symptoms

- Layers split apart.
- Parts break along layer lines.
- Printed brackets fail under relatively light loads.

### Possible Causes

- Nozzle temperature too low
- Excessive cooling
- Moisture
- Poor extrusion
- Print orientation

### What to Try

1. Verify the filament profile.
2. Check nozzle temperature.
3. Review cooling settings.
4. Check for under-extrusion.
5. Consider changing print orientation.
6. Add wall loops where appropriate.

**Remember:** More infill doesn't automatically solve weak layer adhesion.

For functional parts, orientation and wall thickness are often more important.

---

## 💧 5. Wet Filament

### Symptoms

- Popping or crackling during extrusion
- Excessive stringing
- Rough surfaces
- Inconsistent extrusion
- Unexpected deterioration in print quality

### What to Try

- Dry the filament according to its manufacturer's recommendations.
- Store unused filament in a dry environment.
- Use appropriate sealed storage or desiccant when necessary.
- Avoid overheating filament during drying.

PETG can absorb moisture, so filament condition is worth checking when troubleshooting unexplained print defects.

---

## 🐘 6. Elephant's Foot

### Symptoms

The bottom layers of a print bulge outward, making the base slightly wider than intended.

### Possible Causes

- Excessive first-layer compression
- Bed temperature too high
- Insufficient cooling
- First-layer flow issues

### What to Try

1. Verify the correct build plate settings.
2. Review first-layer calibration.
3. Check bed temperature.
4. Use elephant's foot compensation in Bambu Studio when appropriate.
5. Add a small chamfer to the bottom of the model if the design permits.

This problem can be particularly frustrating when printing electronics enclosures with tight-fitting lids.

---

## 🌉 7. Poor Bridges & Overhangs

### Symptoms

- Sagging bridges
- Drooping overhangs
- Rough undersides
- Unsupported material curling upward

### Possible Causes

- Insufficient cooling
- Excessive temperature
- Printing too quickly
- Unsupported geometry
- Poor model orientation

### What to Try

- Review cooling settings.
- Adjust print speed for overhangs.
- Reorient the model.
- Add supports when necessary.
- Consider redesigning the part to reduce unsupported geometry.

Sometimes the best solution is changing the design rather than changing the printer.

---

## 📏 8. Parts Don't Fit Together

### Symptoms

- Lids won't close.
- Screws don't fit.
- PCBs don't align with mounting holes.
- Snap-fit connections are too tight or too loose.

### Possible Causes

- Insufficient model clearance
- Incorrect dimensions
- Material shrinkage
- Elephant's foot
- Flow calibration
- Print orientation

### What to Try

1. Measure the actual printed part.
2. Compare the measurements with the model.
3. Check whether the error is consistent.
4. Review first-layer expansion.
5. Adjust clearances in the design.
6. Print a small test section before reprinting the entire model.

### A Practical Lesson

When designing electronics enclosures, I try to remember that the dimensions in CAD aren't necessarily the dimensions of the finished print.

A little clearance can save a lot of frustration.

---

## 🧵 9. Under-Extrusion & Clogged Nozzles

### Symptoms

- Missing sections of printed walls
- Gaps between extrusion lines
- Thin or inconsistent layers
- Filament stops extruding

### Possible Causes

- Partial nozzle clog
- Filament feed problem
- Incorrect temperature
- Excessive volumetric flow
- Filament contamination

### What to Try

- Verify the correct filament profile.
- Check that filament feeds properly.
- Inspect the nozzle for clogs.
- Reduce printing speed or volumetric flow if necessary.
- Follow Bambu Lab's recommended maintenance procedures.

**Safety:** Allow hot components to cool before handling them. Follow the printer manufacturer's procedures when working with the hotend or extruder.

---

## 🍝 10. Spaghetti Failures

### Symptoms

You expected a finished print.

Instead, you got an impressive collection of plastic noodles.

### Possible Causes

- Print detached from the build plate
- Support structure failed
- Part collision
- Poor first-layer adhesion
- Incorrect slicing or model geometry

### What to Try

1. Inspect the build plate and first layer.
2. Check the model's contact area.
3. Review supports.
4. Look for curled edges or areas where the nozzle may have collided with the print.
5. Consider adding a brim or changing orientation.

If the print failed halfway through, look for evidence of what happened immediately before the failure.

The location of the failure can tell you more than the spaghetti itself.

---

## ↔️ 11. Layer Shifting

### Symptoms

A section of the print suddenly becomes offset from the layers below it.

### Possible Causes

- Nozzle collision
- Mechanical obstruction
- Loose or incorrectly tensioned belts
- Excessive printing speed or acceleration
- Print detaching or curling

### What to Try

- Check for obstructions.
- Inspect the printer's motion system.
- Look for curled or raised print sections.
- Review speed and acceleration settings.
- Follow Bambu Lab's maintenance instructions for the A1.

Avoid adjusting belts or disassembling printer components without following the manufacturer's instructions.

---

## ⚙️ Troubleshooting in Bambu Studio

Before making major changes, I recommend:

1. Confirming the correct printer profile.
2. Confirming the nozzle size.
3. Selecting the correct filament profile.
4. Verifying the build plate configuration.
5. Reviewing the sliced preview.
6. Checking support placement.
7. Printing a small test model.

When diagnosing a problem, change one setting at a time whenever possible.

Otherwise, it's difficult to know what actually fixed it.

---

## 🧪 My Troubleshooting Log

I'll use this section to document problems from actual projects.

| Project | Problem | Solution | Result |
|---|---|---|---|
| Future project | To be documented | To be documented | To be documented |

Over time, this should become one of the more valuable parts of the workshop.

A solution that worked on a real project is usually more useful than a dozen guesses.

---

## 💡 My General Troubleshooting Approach

When something goes wrong, I try to follow a simple process:

**Observe → Identify → Test → Adjust → Print Again**

- Look at the failure before changing settings.
- Start with the most likely causes.
- Test the simplest fix first.
- Change one variable at a time.
- Document what actually worked.

Sometimes the solution is a slicer setting.

Sometimes it's the filament.

Sometimes it's the design.

And sometimes I just made something that looked great in CAD but had absolutely no business being printed that way.

That's how we learn.

---

## Affiliate Disclosure

Some product links on this page are affiliate links. I may earn a commission from qualifying purchases at no additional cost to you. These links help support future Purpose in Practice projects.

---

*Learn it. Build it. Put it into practice.*

**Purpose in Practice**
