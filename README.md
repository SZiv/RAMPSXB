# RAMPSXB
For anyone who does extensive, hardcore, overkill 3D printer work, will typically run out of either stepper motor slots for extruders, MOSFETS for Heaters/fans, or Thermistor pins. The options for this are to either upgrade to an expensive mainboard like a duet, or add on individial drivers for stepper or FET. There isn't really a cheap or easy option. Now there is! RAMPSXB is an expansion board for the popular control board that connects to the AUX and endstop headers like an arduino shield to add functionality to the system. in addition, most components and schematic layouts follow the Reprap Defacto standard, as well as the original RAMPS board, so the thermistors, FETs, microstepping and drivers should all behave as if they were an extension of the RAMPS board itself. Most components are dirt cheap, and the board can be outsourced and assembled with a simple soldering iron. 

RAMPSXB is an expansion board shield for serious 3D printer people that adds an overkill amount of functionality to run high-end extruder systems like the E3D Kraken or Diamond Full Color Hotend: 

- 4 additional Stepper motors (bringing the total to 9; enough to run 6 extruders) 
- 4 additional Thermistor pins
- 4 additional MOSFETs w/ PWM control
- EXP1 and EXP2 headers for a Reprap Full Graphics Smart Controller (With SD Card)
- 4 additional 12V rail pins w/ grounds
- 4 additional 5V rail pins w/ grounds
- 2 steppers have two rows of output pins for driving 2 motors together
- Broken out, preregulated pins for HC-05 Bluetooth Chip
- Isolated input and microcontroller power, so 12V or 24V power can be used for the FETs. 
- Suppression Capacitors on endstops to reduce false positives caused by inductive voltages.
- 1 servo pin (the other 3 were consumed for PWM on the FETs)
- Broken out 12C pins



This comes at the cost of: 
- 3 of the 4 servo pins. 
- Max endstops (there are only min endstops)
- AAAAAAALL the AUX headers (with the exception of 1 digital pin, D40, which is broken out)
- A lot of additional space


If you have questions, feel free to shoot me a message.

Happy printing!

Released under GPL V3



---- Pin Definitions ----

E2 Direction      -  15  
E2 Step           -  19  
E2 Enable         -  63  
E3 Direction      -  2  
E3 Step           -  39  
E3 Enable         -  58  
E4 Direction      -  42  
E4 Step           -  44  
E4 Enable         -  49  
E5 Direction      -  32  
E5 Step           -  47  
E5 Enable         -  57  
Thermistor T3     -  A11  
Thermistor T4     -  A12  
Thermistor T5     -  A10  
Thermistor T6     -  A5  
MOSFET 2          -  4
MOSFET 3          -  5
MOSFET 4          -  6
MOSFET 5          -  45  

HC-05 chip, LCD screen, and SD card follow the standard pinouts



---- Bill of Materials ----  

Part                                      Quantity          Package  

Electrolytic Capacitors, 100uF, SMD         4                 0605  
Electrolytic Capacitors, 10uF, SMD          4                 0405  
Nonpolarized Capacitor, SMD, 0.47uF			3				  0805  
Resistors, SMD, 100k Ohm                    8                 0805  
Resistors, SMD, 10k Ohm                     4                 0805  
Resistors, SMD, 10 Ohm                      4                 0805  
Resistors, SMD, 1.8k Ohm                    4                 0805  
Resistors, SMD, 4.7k Ohm                    4                 0805  
Resistors, SMD, 3.3k Ohm                    1                 0805  
Resistors, SMD, 2.2k Ohm                    1                 0805  
MOSFET, Through-hole, stp55nf06l            4                 TO-220  
LEDs, SMD                                   4                 0805  
Screw Terminals                             5                 3.5mm  
Schurter Fuse Holder                        1                 SH22,5  
PTC Fuse                                    1                
Pin Headers, 1x18, female, 0.1" spacing     1                 N/A   
Pin Headers, 1x8, female, 0.1" spacing      8                 N/A  
Pin Headers, 2x10, female, 0.1" spacing     1                 N/A  
Pin Headers, 2x4, female, 0.1" spacing      3                 N/A
Pin Headers, 1x4, female, 0.1" spacing      2                 N/A
Pin Headers, 1x6, female, 0.1" spacing      3                 N/A  
Pin Headers, 1x1, male, 0.1" spacing        1                 N/A  
Pin Headers, 2x4, male, 0.1" spacing        6                 N/A  
Pin Headers, 1x4, male, 0.1" spacing        3                 N/A  
Pin Headers, 2x5, male, 0.1" spacing        2                 N/A
Pin Headers, 2x2, male, 0.1" spacing        1                 N/A  
Pin Headers, 1x3, male, 0.1" spacing        4                 N/A  
  



