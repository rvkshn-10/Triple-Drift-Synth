# Triple Drift purchasing draft

Checked October 24, 2026. Currency: USD. **The current estimate is $101.37, which exceeds the $65 limit by $36.37. This is not an approved shopping list or a verified delivered quote.** The BOM is populated so the actual circuit requirements and remaining cost problems are visible.

## Prices and estimates

`BOM.csv` uses Part, Qty, Unit, Total, Vendor and Link. Unit and Total are USD. Price status, circuit references and purchase/fit notes are preserved below. Quantity means quantity purchased, rather than the number used. Six resistor values are each budgeted as ten-piece purchases. Every required plastic part is included: one base, one lid, seven knobs, one speaker bridge and one battery pull grip.

Tayda listed prices replace the larger Amazon component packs. Electronics prices are product listing prices, not a completed checkout. Listed prices, uploaded-model quotes and unverified allowances are identified separately in the CSV. Stock, minimum purchase quantities and the total must be checked again at checkout. There are no promotional coupons, free shipping assumptions or prorated kit costs.

The uploaded final STL models produced a JLC3DP quote of $18.16 using 9600 white resin: base $10.85, lid $4.43, seven knobs $2.24, bridge $0.32 and pull grip $0.32. The US country-level shipping estimate was $14.03 for Global Standard Direct Line, 0.54 kg. This was not a final address-level checkout. Changing resin or processing changes the price. Resin is a different manufacturing material from an FDM plastic prototype and its threaded mounting features still require validation.

The $2 PCB line is only a base-price allowance for a five-board batch, not an uploaded Gerber quote. The existing PCB is 100 x 100 mm, two layers, 1.6 mm. An $8 separate PCB shipping allowance is included. JLC documents combined payment for PCB and printing orders, but that does not establish a shared shipping price. Replace both shipping lines with the actual combined or separate checkout charges if available.

JLC's published US policy lists 40% for plastic prints and 35% for PCBs. Reserves of $7.26 and $0.70 are included. Mouser lists a possible 10% speaker tariff, reserved as $0.45. Do not add a tariff twice if the checkout price already includes it. The $8 Tayda shipping/import allowance, $8 Mouser shipping allowance and $7 sales/use-tax reserve are estimates, not supplier quotes or guaranteed ceilings. The other hardware/consumable allowances also require full purchase prices and any shipping before approval.

## Assembly and fit

The circuit has three NE555 timers, one LM386, one diode, 16 resistors, 20 capacitors, seven panel pots, five maintained toggles and one momentary PLAY switch. Panel wires are to be soldered directly to the PCB connector pads to avoid buying headers and mating connectors. This requires careful strain relief. No paid assembly is included. Solder is budgeted; a soldering iron, cutters and meter are assumed borrowed. Buying these tools would increase the total.

The speaker candidate is Same Sky CMS-4065-28SP, 8 ohms, 2 W, 40 mm diameter and 6.5 mm deep, listed at $4.46 by Mouser. Its nominal envelope is compatible with the design's 40 x 8 mm placeholder, but retention, rim geometry and physical fit have not been tested. Tayda's cheaper 57 mm speaker was excluded because it does not match the designed cradle.

Do not order the enclosure yet. The selected B100k pot listing calls for a 7.5 mm mounting hole while the CAD holes are 7.2 mm. Shaft reach, included mounting nuts/washers, switch clearances and printed-knob retention require checks. Several film capacitors have 5 mm lead spacing but larger bodies than the nominal PCB footprints, especially the 1 uF capacitor. Check placement clearances before purchasing or update the footprints and rerun board checks. Screw lengths, head-pocket fit and resin thread strength also need confirmation. No CAD or PCB geometry was changed during this costing pass.

## Reaching $65

The $65 target remains unresolved. The next cost revision needs a smaller or lighter enclosure quote and fewer supplier shipments, with a compatible lower-cost speaker. Any candidate must still include the full purchase quantities, PCB fabrication, every printed part, battery, hardware, consumables, shipping, duties and tax. Do not reduce the total by omitting those costs. A cheaper supplier alone has not established a $65 build.

## Sources

Individual electronics links are in the CSV. Additional sources:

- [JLC US tariff policy](https://jlc3dp.com/help/article/us-tariff-policy-faq)
- [JLC combined-order payment instructions](https://jlc3dp.com/help/article/how-to-combine-orders-for-jlc3dp-and-jlcpcb-products)
- [JLC3DP quoting](https://jlc3dp.com/)
- [JLCPCB base pricing](https://jlcpcb.com/)
- [Mouser 40 mm speaker listings](https://www.mouser.com/en/c/electromechanical/audio-devices/?diameter=40+mm)
- [California sales and use tax rates](https://www.cdtfa.ca.gov/taxes-and-fees/rates.htm)

## Part details

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
- **100nF 100V 5% film capacitor** — Listed price; fit pending. References: C2 C6 C11 C13 C14 C21 C23 C24 C31 C33 C34. A-951; 5mm pitch; verify 7.2mm body clearances against disc footprints
- **10nF 100V film capacitor** — Listed price; fit pending. References: C12 C22 C32. A-559; 5mm pitch; check body clearance
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
- **40mm 8 ohm 2W speaker CMS-4065-28SP** — Listed price; fit pending. References: J2. 40 x 6.5mm; candidate for nominal 40 x 8mm cradle; verify datasheet and retention before ordering
- **Hookup wire and heat-shrink purchase** — Allowance. References: J1-J15 panel wiring. Direct solder to PCB connector pads; no headers or mating plugs purchased
- **9V alkaline battery purchase** — Allowance. Confirm full pack price; no free battery assumed
- **M3 mounting hardware purchase** — Allowance. 4 M3x8 lid; 6 M3x6 PCB/bridge; 7 M3x6 set screws; verify screw depths/head pockets and resin thread strength
- **Feet ribbon cable ties purchase** — Allowance. 4 approx 12mm feet; 10mm-wide pull ribbon; cable ties; full purchase allowance
- **Solder purchase** — Allowance. Self assembly; soldering iron/cutters/meter assumed borrowed; purchasing tools would be extra
- **PCB fabrication batch of 5** — Base-price allowance; no uploaded quote. 100x100mm 2 layers 1.6mm FR4; cost for full batch; no stencil or paid assembly
- **3D print base** — Uploaded-model quote. 9600 white resin; all final STL quantities included; quote subject to review
- **3D print lid** — Uploaded-model quote. 9600 white resin; all final STL quantities included; quote subject to review
- **3D print grip-knob** — Uploaded-model quote. 9600 white resin; all final STL quantities included; quote subject to review
- **3D print speaker-bridge** — Uploaded-model quote. 9600 white resin; all final STL quantities included; quote subject to review
- **3D print battery-pull-grip** — Uploaded-model quote. 9600 white resin; all final STL quantities included; quote subject to review
- **JLC3DP US shipping** — Country shipping estimate. Global Standard Direct Line; 0.54kg; print-only shipping estimate
- **PCB shipping allowance** — Allowance. Separate PCB shipment allowed for; combined payment does not establish shared shipping; replace with actual quote
- **Tayda shipping/import allowance** — Allowance. Actual checkout shipping and any import charges unverified
- **Mouser speaker shipping allowance** — Allowance. No free shipping assumed; replace with checkout quote
- **JLC resin import reserve 40%** — Policy-based reserve. 40% of 18.16 rounded up; remove only if already included at checkout
- **PCB import reserve 35%** — Policy-based reserve. 35% of 2.00; avoid double counting checkout-inclusive duties
- **Speaker tariff reserve 10%** — Listed possible tariff reserve. 10% of 4.46 rounded up; confirm checkout
- **Sales/use tax reserve** — Allowance. Reserve only; exact destination tax and taxable base not quoted; replace at checkout
- **ESTIMATED TOTAL - OVER $65** — Not a delivered quote. Do not order against a $65 cap until revised and checkout verified
