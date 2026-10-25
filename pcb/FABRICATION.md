# PCB source and manufacturing files

Open **TripleDrift.kicad_pro** in the repository root with KiCad 10. The matching schematic is **TripleDrift.kicad_sch** and routed board is **TripleDrift.kicad_pcb**, beside the project file. Footprints are embedded in the PCB; normal KiCad libraries are used for editing. Local preferences and lock files are not required and are not included.

For bare-board quoting, upload **TripleDrift-Gerbers.zip** from this folder. Its contents are also available individually in **manufacturing/**: front/back copper, front/back solder mask, front/back silkscreen, Edge.Cuts, plated-hole drill and non-plated-hole drill files, plus the Gerber job file. The board is 100 x 100 mm, two layers, 1.6 mm FR4. This is a bare-board package, not a factory-assembly order. The circuit requires through-hole soldering and panel wiring.

## Verification

Checked October 24, 2026 using KiCad 10 CLI:

- Electrical rules check: zero errors and warnings under the included project settings.
- Board design rules check: zero reported violations and zero unconnected pads.
- Schematic-to-board parity: zero issues.
- Independent pin/net audit: 141 connected pads match the schematic.

The upload copy's net names, description/datasheet fields and unused LM386 gain-pin net names were synchronized with the schematic. The four mechanical mounting holes are marked board-only. A before/after check confirmed unchanged physical layout, track geometry and connected-net membership. These metadata corrections do not change the enclosure fit. Reports are in **checks/** and list the project-configured ignored checks.

Digital checks do not establish physical part fit or working audio. The purchased capacitor body clearances, print tolerances and final wiring remain untested. The BOM is still a cost estimate and the revised printed parts need a new quote.

## Lower-cost speaker revision

The BOM already selects **Tayda A-4117 / HY57MS0810-H8.4, 57 mm, 8 ohms, 1 W, listed at $0.95**. It replaces the separate Mouser speaker order. It has the same nominal impedance required by the circuit, so no electrical redesign is needed for that substitution. Use the matching **cad/cost-revision/** enclosure and retaining bridge, including its updated grip knobs. Those native F3D, STEP and STL files are in this repository and the Fusion design is saved in Admin Project.
