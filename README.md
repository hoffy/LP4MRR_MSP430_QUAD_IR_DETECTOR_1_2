LP4MRR_MSP430_QUAD_IR_DETECTOR_1_2
==================================

Launchpad for Model Railroading Quad Infrared Detector Project Ver 1.2


Instructions and Notes.txt
Quad Infrared Detector Version 1.2
COPYRIGHT © 2013 S.D. "Hoffy" Hofmeister
http://www.hoffysworld.com
Provided under a Creative Commons Attribution, Non-Commercial Share Alike,3.0
Unported License
TARGETED TO MSP430 LANUCHPAD W/MSP430G2553 PROCESSOR
**** PLEASE READ THIS ENTIRE DOCUMENT BEFORE USING THIS PROJECT DESIGN ****
-----------------------------------------------------------------
This code is designed to control 4 IR Sensors and light 4 independent indicator LEDS
to signal that an object as been detected.
Distance between Tip of Emitter and Tip of Detector has only been tested upto 3.5
Inches under incandescant and floroescant
lighting conditions with no failures. Separation distance may be affected by wire
lengths from the Launchpad.
This Project has been designed to be powered by the USB connection. Consult other
available instructions on how to connect your MSP430 to external power sources
before attempting.
Pin Assignments:
----------------
PIN 1.0 = Cathode of IR Receiver #1 > Anode to Ground
PIN 1.1 = UNASSIGNED - UART
PIN 1.2 = UNASSIGNED - UART
PIN 1.3 = Cathode of IR Receiver #2 > Anode to Ground
PIN 1.4 = Cathode of IR Receiver #3 > Anode to Ground
PIN 1.5 = Cathode of IR Receiver #4 > Anode to Ground
PIN 1.6 = Anode of Indicator LED #1 \
PIN 1.7 = Anode of Indicator LED #2 \ Cathodes to ground
PIN 2.0 = Anode of Indicator LED #3 /
PIN 2.1 = Anode of Indicator LED #4 /
PIN 2.2 = UNASSIGNED
PIN 2.3 = UNASSIGNED
PIN 2.4 = UNASSIGNED
PIN 2.5 = Circuit Power Indicator
PINS 1.1, 1.2, 2.2, 2.3, 2.4 are left unused for integration into other projects.
__________________________________________________________________________________
FILES IN THIS PACKAGE:
----------------------
Quad Infrared Detector Version 1_2_COMPILER_CODE.TXT -- The code of copy and
paste into the Code Coposer Studio Software
Quad Infrared Detector Version 1_2_CODE.PDF -- Color separated PDF version of
code for easier reading
Quad Infrared Detector Version 1_2_schem.PDF -- The Electrical Schematic for this
project
Quad Infrared Detector Version 1_2_Visual.PDF -- A visual representation of how to
wire this project to the MSP430 Launchpad
Insructions and Notes.PDF -- This File
__________________________________________________________________________________
Page 1
Instructions and Notes.txt
COMPONENTS NEEDED FOR THIS PROJECT:
-----------------------------------
Radio Shack Catalog# 276-142 - Infrared Emitter and Detector LED Set or comparable
Radio Shack Catalog# 276-021 - Yellow 5mm LED or comparable -- OPTIONAL
Wire
appropriate insulating material for connections to LEDS ie. Electrical Tape
__________________________________________________________________________________
UNDERSTANDING YOUR COMPONENTS:
------------------------------
What is an Anode and a Cathode?
Imagine the image below is an LED
/\
||
--
|| An LED as two leads that come off of it, one long and one short.
|| The long Lead is the ANODE and the short one is the CATHODE, on many LEDS
you will notice the LED has a flat edge on one side and a
| rounded edge on the other. The flat side is the CATHODE
What is VCC and GND Mean?
VCC is your (POSITIVE Voltage +) connection
GND is your (NEGATIVE - or GROUND) connection
___________________________________________________________________________________
PREPARING YOUR MSP430 LAUNCHPAD FOR THIS PROJECT:
-------------------------------------------------
You will notice many jumpers (Little Black Rectangle Thingys) on the MSP430
launchpad,
beside them you will see white lettering that identifies them.
There are two jumpers located near the edge of the board labeled P1.0, and P1.6
remove these two jumpers. If you are not sure which ones to
remove, connect the launchpad to your computer using the included USB cord. The two
jumpers near the Red and Green flashing LEDS are the jumpers
to remove. Unplug the Launchpad from your computer before removing these jumpers.
____________________________________________________________________________________
CONNECTING YOUR MSP430 LAUNCHPAD TO THE LEDS:
---------------------------------------------
Page 2
Instructions and Notes.txt
Note Anodes for the IR Emitters connect to VCC and Cathodes to GND
**** THE IR DETECTOR LEDS ANODES CONNECT TO GND -- See note below for more detail 1
****
Please read the packaging or datasheets for the Radio Shack # 276-142 Emitters and
Detectors to determine which LED is the Detector and which is
the Emitter.
____________________________________________________________________________________
**** PLEASE TAKE CAREFUL NOTE ****
1 Normally LEDs are connected Anode to (positive +) symbolized as VCC on the
microcontroller and Cathode to (Negative - or GROUND) symbolized
on the microcontroller as GND. The IR Detectors connect differently. **** THE
IR DETECTOR LEDS ANODES CONNECT TO NEGATIVE ****
Consult the Quad Infrared Detector Version 1_2_Visual.pdf file in this package
for a better understanding of these connections.
Page 3
