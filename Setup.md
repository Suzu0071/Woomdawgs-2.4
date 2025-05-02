# Setup
## Beacon
Download beacon things from [here](https://docs.beacon3d.com/quickstart/).
## Wiring

Wiring related is found [here](https://docs.ldomotors.com/en/voron/voron2).

+ The X stepper (on the left) goes into HV-Stepper0. Endstop goes to 
+ The Y stepper (on the right) goes into HV-Stepper1.

+ Left front Z stepper goes to Stepper0.
+ Left back Z stepper goes to Stepper1.
+ Right back Z stepper goes to Stepper2.
+ Right front Z stepper goes to Stepper3.

+ The toolhead board wire goes to CAN and to the PSU.

## Config
1. **Download repository as zip.**
2. **Extract.**
3. **In mainsail/fluidd create corresponding folders.**

<img src="https://raw.githubusercontent.com/Suzu0071/Helper-Repository/refs/heads/main/Configs/create-directory.png" width=500px>

4. **Drag+Drop the files from `downloads` to the printer.** Mainsail doesn't support dropping folders for some reason :x

<img src="https://raw.githubusercontent.com/Suzu0071/Helper-Repository/refs/heads/main/Configs/drop-files.png" width=700px>

Don't forget to change the `printer.cfg`.

## Things to change/tune
+ MCU serials. (In `Main.cfg`)
+ Thermistor types, because idk what you have c:
    + Extruder and bed in `Main.cfg`.
    + Chamber in `Main.cfg`.
+ Probe Z offset. (In `Bed-Related.cfg`)
+ PID tune bed and hotend. (In `Main.cfg`)
+ Tune E-steps. (In `Main.cfg`)