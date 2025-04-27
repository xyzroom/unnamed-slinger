# Design log

## April 27 2025:
- Uploaded V1-test assembly .step files, EXCLUDING HIWIN configurator models for the the MGN12 rails and MGN12H blocks, due to uncertainty about the copyright

## April 20 2025: V1-test final
- Uploaded all finalised V1-test .step files. Reprinted in PETG and installed within SAMLA box
- Can extend frame in Y direction by about 7mm and X by 1 or 2 mm in the new SAMLA boxes.
- Toolhead is basic (no part cooling)
- Z endstop probing is basic (Makerstop endstop)
- A/B motor cooling designed but not installed
- Y motor cooling not yet designed
- Skipping steps on Y, either due to thermal expansion or motors running too hot
- Y axis redesign for V2: remove 1 linear rail. There are three locations on the Y carriage plate where the remaining MGN12 can be mounted

## April 6 2025:
- Created 'V1-test', beginning to upload 'final' .step files
- Updated Y motor mounts

## April 1 2025
- One week sprint: First version assembled in PLA, excluding motor cooling fans and SAMLA box
- Electronics working without issue, aside from a defective heated bed MOSFET which I replaced
- Layer shifting due to bad belt tensioning on Y axis. Otherwise printer is silent and prints well
- Comments and next changes:
  - Y motor mounts: Change holes to slots so the belt tension can be even higher
  - Wiring and Bowden tube to go to the front of the printer to avoid interference with the Z endstop and XZ belts
  - Sensorless homing (X and Y): Concerning crashes/sensitivities, especially due to temperature variations. Replace with endstops in V2
  - Y carriage: Heating pad thicker than expected and in contact with Y belt holder, causing deformation. Currently spaced by 18mm silicon spacers with extra 1mm printed washer underneath. Also the silicon spacers interfere with the heating pad and are not flush with the bed - does not appear to be an issue. Very minimal increase in binding towards one end of Y axis (bent rail?).
  - XZ motor mounts: Motor wire connectors are so close to the 1515 extrusion that one wire is slightly pinched. Not urgent
  - Volcano clone: Thermistor and heater cartridge wires must be bent a concerning amount

## March 14 2025
- Increased spacing around Y motors by 1mm for airflow
- Edited Y motor mounts and Y carriage belt holder to be more sensible CAD-wise

## March 13 2025
- Started repo, upload images and files later
- Parts on their way
- Designing part cooling for V2
- Figuring out Bowden extruder placement

- Assessing motor cooling options for Y axis steppers
- Assessing air circulation options under heated bed
- Considering static part cooling fans on X axis behind toolhead
