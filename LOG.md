# Design log

## April 1 2025
- First version has been assembled in PLA, excluding motor cooling fans and SAMLA box
- Printer is to be reprinted in PETG and completely reassembled, so wiring is a mess right now
- Klipper/Mainsail on BTT Pi and SKR Pico
- Encountered and resolved defective heated bed MOSFET
- Except layer shifting on Y axis, print quality is good. Printer is very quiet
- Comments and next changes:
  - Y motor mounts: Change holes to slots so the belt tension can be even higher. Current configuration, belt tension too loose, causing layer shifting in the Y direction (belt skipping over pulleys).
  - XZ motor mounts: Motor wire connectors are so close to the 1515 extrusion that one wire is slightly pinched (not a big deal)
  - Volcano clone: Heatbreak bent, replace. Thermistor and heater cartridge wires at significant bend angle.
  - Toolhead wiring: Bowden tube goes to the front, deciding on whether wiring to back or front
  - Heated bed wiring: Deciding whether wiring to back or front
  - Z endstop: Fine. If heated bed wiring goes to the back, may interfere.
  - Sensorless homing (X and Y): Install non-structural, pliable parts to collide against rather than damage the system.
  - Y carriage assy: Silicon heater thicker than expected and possibly in contact with Y belt holder. Currently spaced upwards by 1mm printed washer underneath the 18mm silicon spacers. Also the silicon spacers interfere with the heating pad and are not flush - does not appear to be an issue. Very minimal binding on one end of Y axis (belt rail?).
  - X carriage: Loose ends of XZ belts in way, restricting full 120mm X range. Leave for now. 
  - XZ belt: Belt tension is high, Z axis falls slowly. Toolhead easily moved by hand in 45 degree directions but not as easily in X and Z.

## March 14 2025
- Increased spacing around Y motors by 1mm for airflow
- Edited Y motor mounts and Y carriage belt holder to be more sensible CAD-wise
- Y motor cooling (blowers towards motors, drawing air from under the bed) replaced by axial fans blowing upwards, drawing air from motors

## March 13 2025
- Started repo, upload images and files later
- Parts on their way
- Designing part cooling
- Figuring out Bowden extruder placement
- Assessing motor cooling options for Y axis steppers - currently just having 5015 blow at side
- Assessing air circulation, especially under heated bed (distribute heat rather than gather near motors)
- Considering static part cooling fans on X axis behind toolhead
