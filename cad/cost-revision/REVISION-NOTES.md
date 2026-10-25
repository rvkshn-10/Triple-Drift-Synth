# Lower-cost purchased-part revision

October 24, 2026. Fusion document: **Triple Drift - Cost revision - 57mm speaker**, in **Admin Project**. The original completed Phase 3 document was preserved.

## Purchased parts and fit changes

- Selected Tayda A-4117, HY57MS0810-H8.4: 57 mm, 8 ohm, 1 W speaker, listed at $0.95. Supplier drawing gives 57 +/- 0.2 mm diameter, 8.4 mm nominal depth and a 17.2 mm magnet. The CAD reserves a 57.2 mm diameter x 8.6 mm deep envelope. It has three radial locating stops around a 58.2 mm clearance diameter, a rounded diagonal bridge and a nine-slot grille. A nominal 0.4 mm soft pad against the rear magnet accommodates depth variation. Terminal orientation and soldered wire routing require physical verification.
- Voice columns moved from x=25/60/95 mm to x=25/58/90 mm. Control holes, purchased-part envelopes, knobs, legends, scales and grouping borders were adjusted together. Overall case remains 160 x 130 x 47 mm.
- The selected round-shaft pots retain their original resistance values and tapers. Panel holes widened from 7.2 to 7.7 mm. Three blind 3.2 mm anti-rotation pockets were added for the pitch pots' tabs. Knob bottom height changed to z=50.8 mm to accommodate the selected 15 mm shaft reach. B100k body drawing: 16.9 mm body diameter, 6 mm shaft, M7x0.75 bushing and 6.5 mm threaded length. Remaining pots retain conservative body and lug envelopes rather than exact supplier solids.
- Tayda A-4567/MTS-102 toggle body and terminal envelopes were modeled from the supplier drawing: 13.2 x 7.9 x 9.5 mm body, 4 mm terminals, 6 mm bushing. The existing 6.5 mm panel openings remain. The actual retaining washer/tab installation must be checked.
- Tayda A-6454/DS-227 PLAY button drawing requires a 12.5 mm cutout. CAD now uses 12.7 mm clearance. PLAY moved upward to z=32.5 mm to clear the PCB with the deeper body and terminals. The front PLAY legend moved beside the button to clear its 16.5 mm flange.
- The final live knob revision replaces the tapped 2.6 mm set-screw pilot with a 3.3 mm clearance hole and a bottom-loading M3 nut channel, 2.7 x 5.9 x 8.95 mm. It uses seven M3x8 headed screws and seven M3 nuts from the existing kit. Check leftover quantities, nut dimensions and head diameter/height before printing. Design check assumes screw heads fit within a 14 mm rotation radius, giving 4 mm minimum separation between neighboring knob sweep envelopes. Nylon screws should be tightened gently.

## Validation and export status

The final live knob revision passed a digital solid-interference check across 115 bodies with no printed-part collisions. Before the knob revision, the 456-entry model also had no feature errors/warnings and exported to native F3D, STEP and five STL files. These checkpoint meshes were checked for closed two-face edge connectivity, positive signed volume and flat-bed orientation.

**The currently exported files are the 456-entry checkpoint, before the reusable-M3 knob revision.** The live knob revision has 461 timeline entries and returned a successful save to the separate Admin Project document. Fusion stopped responding during its final export. Do not use the checkpoint grip-knob STL as the final reusable-M3 knob. Native exports and latest cloud-version verification remain pending. The source modification scripts are in the task workspace, not an indication that an exported file has been validated.

No parts have been ordered, assembled or sound-tested. Print tolerances, resin thread strength, soft pad compression, actual screw fit and wiring service clearance still require physical checks. The larger speaker and switch changes do not change the electrical circuit or PCB connections.

## Sources

- [Speaker listing](https://www.taydaelectronics.com/hardware-tools/speakers/mylar-speaker-8-ohm-1w.html)
- [Speaker drawing](https://www.taydaelectronics.com/datasheets/files/HY57MS0810-H8.4.pdf)
- [Pitch pot listing](https://www.taydaelectronics.com/100k-ohm-linear-taper-potentiometer-with-solder-lug-shaft-dia-6mm.html)
- [Pitch pot drawing](https://www.taydaelectronics.com/datasheets/files/A-5606.pdf)
- [Toggle drawing](https://www.taydaelectronics.com/datasheets/files/A-4567.pdf)
- [PLAY button drawing](https://www.taydaelectronics.com/datasheets/files/A-6454.pdf)
