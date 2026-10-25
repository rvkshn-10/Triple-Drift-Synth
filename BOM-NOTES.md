# Triple Drift purchasing draft

Checked October 24, 2026. Currency: USD. **The current estimate is $101.37, which exceeds the $65 limit by $36.37. This is not an approved shopping list or a verified delivered quote.** The BOM is populated so the actual circuit requirements and remaining cost problems are visible.

## Prices and estimates

`BOM.csv` preserves the original six columns and adds price status, circuit references and purchase/fit notes. Quantity means quantity purchased, rather than the number used. Six resistor values are each budgeted as ten-piece purchases. Every required plastic part is included: one base, one lid, seven knobs, one speaker bridge and one battery pull grip.

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
