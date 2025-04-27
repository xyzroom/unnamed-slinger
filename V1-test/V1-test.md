# V1-test summary

![front image](Renders/1.png)
![front image](Photos/01.png)

## Y carriage plate
I had this laser cut from 4mm thick 1060 aluminium

## Printed parts
- .step files have been provided
- Supports are unnecessary, but parts are not necessarily in the correct print orientation
- Print in 0.1mm or 0.2mm layer height
- Inner/outer perimeter order. Do not do outer/inner if seams affect the accuracy of small holes
- There are no circular overhangs but bridging capability is necessary. Consider turning off 'thick bridges'

## Fixtures
- M3 screws, most of which are 2mm button heads
- Some brackets need M4

## CAD information
- In the assembly file, MGN12 rails and MGN12H blocks have been removed
- Fixtures may not be modelled accurately, to the correct lengths. Also add and remove spacers/washers where needed

## First iteration summary:
- Basic toolhead (no part cooling)
- Motor cooling not installed

## Issues:
- Skipping steps on Y. Either binding due to thermal expansion with the 2 linear rails, or motors running too hot
- Inconsistent sensorless homing on X/Y due to significant temperature range

## Changes for V2:
- Add endstops on X and Y axes
- Design Y axis motor cooling
- Redesign Y axis to use only 1 linear rail. (There are three locations on the Y carriage plate to mount the MGN12)
- Design part cooling on the toolhead
- Design row of part cooling fans behind the X axis
- Design air circulation fans and carbon filter