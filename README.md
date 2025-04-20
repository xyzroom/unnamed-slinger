# unnamed-slinger

# Overview
- This is a work-in-progress CoreXZ bedslinger 3D printer that is designed to be fully enclosed within a 38x28x28 cm^3 22L IKEA SAMLA storage box.
- The electronics and filament spool are to be housed within a separate SAMLA storage box.

# Summary of components
- 1515L extrusions (NOT Makerbeam 1515 extrusions) and slider nuts, all-bracketed assembly
- 5x 170mm MGN12H, with 2 on each axis except X
- Build footprint of (120mm)^2, Z height not quite at 120mm, can theoretically squeeze there with compromises
- Uses 23.5mm NEMA17 pancakes, which I am in excess of. There are two on the Y axis.
- V6 Volcano Bowden

# Roadmap
- Get printer working
- Slap on a bunch of fans and get enclosure working
- Slap on a bunch of temperature sensors everywhere
- Air filter inside

# Rationale, theory, aims
- Print quality: Smaller printers have lower moving masses and components are more likely to be flat/square/straight.
- Heating: Small, enclosed printers are quick to heat up. A highly even, warm chamber temperature should assist greatly with part quality and strength.
- Ease of travel/modding/general smoothness: Typical enclosed printers either have massive enclosures, are built into their enclosures or have their enclosures built around them. This is inconvenient for both travel and for modding. My design is essentially a printer which can be put inside and taken outside of a clear plastic box.
- Genuinely enclosed: Apart from a notch in the lid for wiring, this has the potential to be actually airtight. Pollutants and heat kept mostly inside -- Open the box outdoors to release harmful emissions.
- Separate printer, electronics and filament into modular system: For example, it is a very popular storage solution to place 4 filament spools in a 22L SAMLA.
- Multiple motors on every axis: I did not wish to purchase new steppers as I had many pancake steppers lying around. I could do somethign like a AWD mini CoreXY, or in this case, a CoreXZ bedslinger with 2 motors on the Y axis. CoreXZ is not really a great motion system in theory, but it should be good enough (?). I chose it due to its symmetry/simplicity, ability to meet space requirements and nature in that both AB motors are involved in every X travel move.
- Separate X and Y: Though not off the table, it is generally harder to vary the toolhead design for something like a CoreXY printer, because of space constraints in every direction. Whereas for this bedslinger, I can offset the entire XZ axis along Y if desired.

# Uncertain:
- Unsure about whether circulation is good or bad. I would do circulation to maintain even temperature and prevent hot spots, but apparently this may achieve the opposite effect.

# Potential issues
- General weight imbalance on X axis
- Overheating of motors