# Manufacturing Injection Molds with an MSLA 3D-Printer

In this documentation, you will learn how to 3D-print your own injection mold designs with an MSLA printer.  
The focus will be on how this is possible with the machines available at the **OpenLab in Hamburg**.  
However, you can still follow this guide if you are using different machines and apply our findings to your own work environment.  

We will work with the mold design provided in this repo.  
If you want to learn how to design your own mold, please refer to the design guide in this repo (not yet provided).  

---

## Choosing the Right Resin

When manufacturing injection molds, the choice of resin is critical. Not all resins are suitable—your resin must be:

- **High-temperature resistant** (to withstand the molten plastic during injection).  
- **Tough and durable** (to resist cracking under clamping pressure).  
- **Low shrinkage** (to maintain dimensional accuracy).  

Recommended resins include (non-exhaustive):  

- **Siraya Tech Sculpt – High-Temperature Resistant Resin** – strong and heat-resistant, ideal for injection molding.  
- **Phrozen Engineering Rigid Ceramic Pro** – high-temperature resin suitable for injection molds.  

---

## Printing Process with MSLA Resin Printers

The general workflow for resin printing looks like this:

1. **Prepare the 3D Model**  
   - Use CAD software to design (or modify) your mold.  
   - Export the model as an STL file.  

2. **Import into the Slicer**  
   - We are using **Vlare Slicer**, which is specific to our machine:  
     **Peopoly Phenom XXL V2**.  
   - In the slicer, configure layer thickness, exposure times, orientation, and supports.  

3. **Slice and Export**  
   - Save the sliced file in the correct format for your printer.  
   - Transfer it to the printer (via USB).  

4. **Prepare the Printer**  
   - Fill the resin vat with the chosen resin.  
   - Level the build plate if necessary.  

5. **Print the Mold**  
   - Start the print and monitor the first layers to ensure adhesion.  
   - In this case, monitoring means listening for a slight *“snap”* sound when the printer lifts the build plate—this indicates good adhesion.  

6. **Post-Processing**  
   - Wash the print (in IPA or a suitable alternative).  
   - Cure the print under UV light.  
   - Lightly sand or finish surfaces as needed for mold quality.  

---

## Finding the Right Print Settings

Resin settings vary depending on the printer, resin brand, and part geometry. To dial in optimal parameters:

- Start with the manufacturer’s recommended settings.  
- Perform **resin calibration test prints** to fine-tune:  
  - Exposure times  
  - Layer heights  
  - Support density  
  - Lift speeds  

We recommend using a resin calibration model such as the **Photonsters Resin Exposure Finder**:  
👉 [Download calibration model](https://www.thingiverse.com/thing:6023738)  

This will help you systematically adjust and lock in the best settings for strong, precise molds.  

For a detailed walkthrough on how to use this calibration model correctly, follow this [guide](https://3dprinterly.com/how-to-calibrate-resin-3d-prints-testing-for-resin-exposure/).  

---

## Tips & Tricks for Printing Injection Molds

This section provides practical advice to help you get the best results when printing molds.

### Learning Resources
- 🎥 [How resin printing works](https://www.youtube.com/watch?v=pbYAhjASGFY&t=414s)  
- 🎥 [How to calibrate your resin](https://www.youtube.com/watch?v=yhWyQPS6qmQ)  
- 🎥 [Common mistakes in resin printing](https://www.youtube.com/watch?v=vUhc_F2-7YA&t=77s)  

### Specific Printing Techniques for Molds
- **Model orientation**:  
  Many guides suggest printing at an angle (typically 20–30°) to reduce suction forces. While this can help prevent failures, angled prints require supports that may damage mold surfaces.  
  Instead, place the mold **flat, with the smallest surface on the build plate** to minimize supports.  
  ⚠️ Important: Never place the inside (cavity) of your mold against the print bed—this will negatively affect surface quality.  

- **Solid molds**:  
  Print the mold as a solid object whenever possible. This increases strength and allows it to withstand injection forces.  

- **Increase bottom layers & exposure time**:  
  Ensures strong adhesion of the mold base to the build plate.  

- **Support placement**:  
  Add supports only on non-critical surfaces to reduce post-processing and avoid damaging functional mold areas.  
