# RAMPSXB
For anyone who does extensive, hardcore, overkill 3D printer work, will typically run out of either stepper motor slots for extruders, MOSFETS for Heaters, or Thermistor pins. The options for this are to either upgrade to an expensive mainboard like a duet, or add on individial drivers for stepper or FET. There isn't really a cheap or easy option.

RAMPSXB is an expansion board shield for the RAMPS control board that adds an overkill amount of functionality to run high end extruder systems like the E3D Kraken or Diamond Full Color Hotend: 

- 4 additional Stepper motors (bringing the total to 9; enough to run 6 extruders)
- 4 additional Thermistor pins
- 4 additional MOSFETs 
- A microSD Card slot
- 4 additional 12V rail pins,
- A 3.3V pin (for Bluetooth HC-05 chips)
- A real fuse
- Isolated input and microcontroller power, so 12V or 24V power can be used for the FETs. 

This all comes at the cost of AUX 2, 3, and 4, so this cannot be used with an LCD screen. In addition, due to a lack of PWM pins, the FETs can only be used in Bang Bang Control. See the full size RAMPSXB version for PWM control.

Happy printing!

Released under GPL V3
