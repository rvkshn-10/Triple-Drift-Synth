# Triple Drift purchasing draft

Updated October 24, 2026. Currency: USD. **The revised estimate is $85.41, down $15.96 from $101.37, but still $20.41 over the $65 limit. This is not a verified delivered quote.** It assumes enough matching screws and nuts remain in the existing M3 kit. The revised CAD still requires a new printing quote.

`BOM.csv` keeps the same display order with Half Life-compatible headers: Item, Qty, Cost/item, Total Cost, Supplier and link. Cost/item means cost per purchased unit in USD. Full purchase quantities are charged. Prices were restored from the last good Git commit after a Half Life sync wrote imported zeros back to the repository. The standalone summary row and duplicate zero shipping summary were removed so they are not imported as additional parts. The sum of the 43 cost rows remains $85.41. Resistors and ceramic capacitors are budgeted in ten-piece purchases. Reused parts have zero new purchase cost and stay visible in the list.

## Changes selected by total cost

- The speaker is now Tayda A-4117 / HY57MS0810-H8.4, 57 mm, 8 ohms, 1 W, listed at $0.95. It replaces the $4.46 Mouser speaker, $8 separate shipping allowance and $0.45 speaker tariff reserve. The existing $8 Tayda shipping/import allowance remains unverified and must cover the revised order.
- Keep six 100 nF film capacitors for C11/C21/C31 timing and C14/C24/C34 audio coupling. Replace C2/C6/C13/C23/C33 bypass capacitors with 100 nF ceramic capacitors. Buy ten at the listed $0.01 each and use five. The three 10 nF control-pin bypass capacitors C12/C22/C32 also become ceramics, bought as ten at $0.01 each. These changes save $0.50 after rounding full line purchases. Supplier category lists 3 mm lead spacing; carefully form the leads for the PCB's 5 mm holes without stressing the ceramic body. Electrical values and voltage ratings remain suitable for the 9 V circuit. No schematic or PCB edits were made.
- Reuse ten matching M3 mounting screws: four M3x8 for the lid and six M3x6 for PCB/bridge. Reuse seven M3x8 headed screws and seven M3 nuts for the revised knobs. This removes the former $4 hardware purchase allowance. Check actual leftover counts, head dimensions and nut thickness before printing. The prior keyboard BOM identifies a nylon fastener kit, so metal set screws are no longer assumed to be included.
- Add $0.50 as an unquoted purchase allowance for thin compliant speaker-pad material. This is not a confirmed retail pack price.

Amazon Prime was considered. The checked 40 mm speaker two-pack was $5.99 with advertised free Prime delivery, and the 555/LM386 IC assortment was $8.10. The selected speaker and ICs from Tayda total $2.55 before shipping, compared with $14.09 for those two Amazon packs. Since other components still require the Tayda order, switching just these parts to Amazon adds $11.54 in merchandise cost without eliminating that shipment. No separate Prime subscription cost is charged because the user already has Prime. Other unselected Amazon packs are not represented as verified cheapest options.

## CAD status

A separate **Triple Drift - Cost revision - 57mm speaker** document was created in **Admin Project**. The original completed Phase 3 design was preserved. The revision adds the larger speaker locator/diagonal bridge/grille, repositions the voice controls and legends, widens pot holes to 7.7 mm and adjusts knob height for 15 mm pot shafts. The selected DS-227 PLAY switch uses a 12.7 mm clearance opening and is raised to avoid the PCB. The knobs now use captive M3 nuts instead of tapped resin set-screw holes.

The completed 461-entry revision is saved in Admin Project and passed the 115-body digital interference check with no printed-part collisions. Its native F3D archive was reopened in Fusion with the final M3 nut-channel knob features present and no feature errors or warnings. Updated F3D, STEP, five STL files and verification reports are in cad/cost-revision. All STL meshes passed closed-edge, positive-volume and flat-bed checks. Physical fit, wiring, resin durability, sound and assembly have not been tested. No parts have been ordered.

## Fabrication and delivered-cost assumptions

All five plastic part types remain included: base x1, lid x1, knobs x7, retaining bridge x1 and battery pull grip x1. The printing line values are **prior-geometry price allowances**, not quotes for the revised files. The former quote was $18.16 for 9600 white resin. Its country-level print shipping estimate was $14.03. New model upload, supplier review and address-level checkout are still required.

PCB fabrication is a $2 base-price allowance for a five-board batch of 100 x 100 mm, two-layer, 1.6 mm boards. It is not an uploaded Gerber quote. The $8 separate PCB shipping allowance remains until an actual quote replaces it. JLC supports combined payment, but shared shipping or a shipping saving has not been established.

The $8 Tayda shipping/import allowance, $7 sales/use-tax reserve and hardware/consumable allowances are unquoted estimates and may be insufficient. The JLC resin reserve of $7.26 and PCB reserve of $0.70 follow its published 40% plastic/35% PCB policy using the old printing allowance and PCB base price. Replace reserves with actual charges and avoid counting duties twice when checkout already includes them. No import charges are assumed waived because an order is small.

Self-soldering is assumed. Wire is soldered directly to PCB connector pads, avoiding headers and mating plugs. Wire/heat-shrink, battery, solder, feet/ribbon/ties remain purchase allowances because leftover quantities were not confirmed. Soldering iron, cutters and meter are assumed borrowed. Purchasing tools or assembly services would increase the total.

## Remaining fit checks

The capacitor body clearances, especially the 1 uF film part, still need checking against PCB footprints. Pot mounting hardware and all shaft/bushing tolerances need physical verification. The speaker drawing informed its CAD envelope, but terminal position, the soft pad and wiring bends require an actual fit test. The existing M3 kit must contain suitable leftover screws and nuts; the zero-cost reuse rows are conditional on that stock.

## Sources

- [Speaker and $0.95 price](https://www.taydaelectronics.com/hardware-tools/speakers/mylar-speaker-8-ohm-1w.html)
- [Speaker supplier drawing](https://www.taydaelectronics.com/datasheets/files/HY57MS0810-H8.4.pdf)
- [Ceramic capacitor prices](https://www.taydaelectronics.com/capacitors/ceramic-disc-capacitors/test-group-2-caps.html)
- [Pitch pot dimensions](https://www.taydaelectronics.com/datasheets/files/A-5606.pdf)
- [Toggle dimensions](https://www.taydaelectronics.com/datasheets/files/A-4567.pdf)
- [PLAY button dimensions](https://www.taydaelectronics.com/datasheets/files/A-6454.pdf)
- [Amazon speaker comparison](https://www.amazon.com/dp/B0GR43H68T)
- [Amazon IC assortment comparison](https://www.amazon.com/dp/B08JTM2SMJ)
- [JLC US tariff policy](https://jlc3dp.com/help/article/us-tariff-policy-faq)
- [JLC combined-order payment instructions](https://jlc3dp.com/help/article/how-to-combine-orders-for-jlc3dp-and-jlcpcb-products)
- [California sales and use tax rates](https://www.cdtfa.ca.gov/taxes-and-fees/rates.htm)

## Unchanged part details


- **NE555P DIP-8 timer** — Listed price. References: U1 U2 U3. A-249
- **LM386N-1 DIP-8 amplifier** — Listed price. References: U4. A-994; amplifier is on PCB; no extra module
- **1N5817 Schottky diode** — Listed price. References: D1. A-159
- **22 ohm 1/4W resistor** — Listed price. References: R1. Buy 10; use 1; full purchase quantity charged
- **10 ohm 1/4W resistor** — Listed price. References: R4. Buy 10; use 1; full purchase quantity charged
- **1k ohm 1/4W resistor** — Listed price. References: R3 R11 R21 R31. Buy 10; use 4; full purchase quantity charged
- **4.7k ohm 1/4W resistor** — Listed price. References: R12 R22 R32. Buy 10; use 3; full purchase quantity charged
- **10k ohm 1/4W resistor** — Listed price. References: R2 R13 R23 R33. Buy 10; use 4; full purchase quantity charged
- **100k ohm 1/4W resistor** — Listed price. References: R14 R24 R34. Buy 10; use 3; full purchase quantity charged
- **470uF 16V radial capacitor** — Listed price. References: C1 C3. A-4521; 8mm diameter; 3.5mm pitch
- **1uF 100V film capacitor** — Listed price; fit pending. References: C4. A-4412; 5mm pitch; body 7.2 x 6 x 11mm; thicker than nominal footprint
- **10uF 50V radial capacitor** — Listed price. References: C5. A-6985; 50V exceeds required 16V; 5mm diameter; 2mm pitch
- **220uF 25V radial capacitor** — Listed price. References: C7. A-8403; 25V exceeds required 16V; verify lead pitch
- **47nF 100V film capacitor** — Listed price; fit pending. References: C8. A-563; 5mm pitch; check body clearance
- **B100k linear 6mm round shaft pot** — Listed price; fit pending. References: RV1 RV2 RV3. A-5606; pitch; mounting specification 7.5mm versus CAD 7.2mm; fit correction needed
- **A100k log 6mm round shaft pot** — Listed price; fit pending. References: RV4 RV5 RV6. A-1650; voice levels; confirm nuts/washers included and shaft reach
- **A10k log 6mm round shaft pot** — Listed price; fit pending. References: RV7. A-1649; master volume; confirm nuts/washers included
- **Mini SPDT ON-ON toggle** — Listed price; fit pending. References: SW1 SW2 SW3 SW4 SW6. A-4567; wire COM and one outer terminal as SPST; insulate unused terminal; verify switch orientation
- **12mm normally-open PLAY button** — Listed price; fit pending. References: SW5. A-6454; DS-227 red; confirm mounting and body clearance
- **9V battery snap** — Listed price. References: J1. A-6676; 15cm leads
- **Hookup wire and heat-shrink purchase** — Allowance. References: J1-J15 panel wiring. Direct solder to PCB connector pads; no headers or mating plugs purchased
- **9V alkaline battery purchase** — Allowance. Confirm full pack price; no free battery assumed
- **Feet ribbon cable ties purchase** — Allowance. 4 approx 12mm feet; 10mm-wide pull ribbon; cable ties; full purchase allowance
- **Solder purchase** — Allowance. Self assembly; soldering iron/cutters/meter assumed borrowed; purchasing tools would be extra
- **PCB fabrication batch of 5** — Base-price allowance; no uploaded quote. 100x100mm 2 layers 1.6mm FR4; cost for full batch; no stencil or paid assembly
- **PCB shipping allowance** — Allowance. Separate PCB shipment allowed for; combined payment does not establish shared shipping; replace with actual quote
- **Tayda shipping/import allowance** — Allowance. Actual checkout shipping and any import charges unverified
- **PCB import reserve 35%** — Policy-based reserve. 35% of 2.00; avoid double counting checkout-inclusive duties
- **Sales/use tax reserve** — Allowance. Reserve only; exact destination tax and taxable base not quoted; replace at checkout
