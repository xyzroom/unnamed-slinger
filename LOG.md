# Design log

## April 20 2025:
- Uploaded all V1-test .step files.
- Toolhead is basic (no part cooling)
- Z endstop probing is basic (Makerstop endstop)
- Can extend frame in Y direction by about 7mm and X by 1 or 2 mm in the new SAMLA boxes.
- Lacks Y motor cooling for now (too lazy to wire).
- Skipping steps on Y, either due to thermal expansion or motors running too hot. I haven't installed Y motor cooling yet.

## April 6 2025:
- Created 'V1-test', beginning to upload 'final' .step files
- Modified and uploaded motor mounts, reprinted in PETG

## April 1 2025
- One week sprint: First version has been assembled in PLA, excluding motor cooling fans and SAMLA box
- Updated parts to be reprinted in PETG and printer to be reassembled, so wiring management is intentionally lacklustre.
- Klipper/Mainsail on BTT Pi and SKR Pico with sensorless homing on X/Y working. Resolved defective heated bed MOSFET issue.
- Aside from layer shifting due to bad belt tensioning on Y axis, print quality is good. Printer is very quiet
- Comments and next changes:
  - Y motor mounts: Change holes to slots so the belt tension can be even higher. Current configuration, belt tension too loose, causing layer shifting in the Y direction (belt skipping over pulleys).
  - XZ motor mounts: Motor wire connectors are so close to the 1515 extrusion that one wire is slightly pinched. This is not a big deal, but a notable comment.
  - Volcano clone: The heatbreak is bent from me dropping it and needs to be replaced. Thermistor and heater cartridge wires at bent at significant angles, which is concerning.
  - Z endstop: Adjustment works fine, but requires Z axis to be homed and held in place via the motors, since the Z axis falls. The Z endstop may interfere with the heated bed wiring if said wiring goes to the back of the printer.
  - Toolhead wiring: Bowden tube goes to the front, where the extruder is. I am deciding on whether to bring wires to the front or the back. Bringing to the back may cause interference with the XZ belts.
  - Sensorless homing (X and Y): Concerning crashes/sensitivities. Install non-structural, pliable parts to collide against rather than damage the system.
  - Y carriage assy: Heating pad thicker than expected and possibly in contact with Y belt holder. Currently spaced by 18mm silicon spacers with extra 1mm printed washer underneath. Also the silicon spacers interfere with the heating pad and are not flush with the bed - does not appear to be an issue. Very minimal increase in binding towards one end of Y axis (bent rail?).
  - X carriage: Loose ends of XZ belts in way, restricting full 120mm X range. Leave for now. 
  - XZ belt: Belt tension is high, Z axis falls slowly. Toolhead easily moved by hand in 45 degree directions but not as easily in X and Z directions.

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
