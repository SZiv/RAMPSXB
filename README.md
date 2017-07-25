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

This all comes at the cost of AUX 2, 3, and 4, so this cannot be used with an LCD screen. In addition, due to a lack of PWM pins, the FETS can only be used in bang-bang mode. There are plans in the future of consuming the Servo Pins and Aux 1 in order to make all the FETS PWM, and possibly free up enough pins to put the controller back in place, but to save board space, this is the first revision.

Happy printing!

Released under GPL V3



---- Pin Definitions ----

E2 Direction      -  31
E2 Step           -  29
E2 Enable         -  27
E3 Direction      -  41
E3 Step           -  39
E3 Enable         -  43
E4 Direction      -  37
E4 Step           -  35
E4 Enable         -  33
E5 Direction      -  32
E5 Step           -  47
E5 Enable         -  45
Thermistor T3     -  A11
Thermistor T4     -  A12
Thermistor T5     -  A10
Thermistor T6     -  A5
MOSFET 2          -  25
MOSFET 3          -  23
MOSFET 4          -  17
MOSFET 5          -  16
SD CS             -  53


---- Bill of Materials ----

Part                                      Quantity          Package
Electrolytic Capacitors, 100uF, SMD         4                 0605
Electrolytic Capacitors, 10uF, SMD          4                 0405
Resistors, SMD, 100k Ohm                    8                 0805
Resistors, SMD, 10k Ohm                     4                 0805
Resistors, SMD, 10 Ohm                      4                 0805
Resistors, SMD, 1.8k Ohm                    4                 0805
Resistors, SMD, 4.7k Ohm                    4                 0805
Resistors, SMD, 3.3k Ohm                    1                 1206
Resistors, SMD, 2.2k Ohm                    1                 1206
MOSFET, Through-hole, stp55nf06l            4                 TO-220
LEDs, SMD                                   4                 0805
Screw Terminals                             5                 3.5mm
Schurter Fuse Holder                        1                 SH22,5
Fuse                                        1                 22x5
Pin Headers, 1x18, female, 0.1" spacing     1                 N/A
Pin Headers, 1x8, female, 0.1" spacing      8                 N/A
Pin Headers, 2x10, female, 0.1" spacing     1                 N/A
Pin Headers, 2x4, female, 0.1" spacing      1                 N/A
Pin Headers, 1x1, male, 0.1" spacing        1                 N/A
Pin Headers, 2x4, male, 0.1" spacing        2                 N/A
Pin Headers, 1x4, male, 0.1" spacing        4                 N/A


