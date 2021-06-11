===============================================================================================================================
INTRO
===============================================================================================================================
This file contains all the important information needed to set up my 8x8 LED Matrix Car Display. 

First off, this display was intended to be mounted and displayed through the inside of a car’s window. Depending on where you live, this may be a reason for a cop to give you a ticket, use at your own risk!! Although this can be used on a car, it surely doesn’t need to be. 

If there is someone out there who actually is using anything from the project and has questions for me, I'll include my email at the bottom of this README. (also feel free to email me if this was helpful to you as it would mean a lot to me to see someone who liked my project) 


===============================================================================================================================
OVERVIEW
===============================================================================================================================
This project uses components (listed on components list) to display scrolling text on an 8x8 led matrix. This project uses an Arduino as the brains connected to a Bluetooth module. 

A smartphone can be connected to the Bluetooth module, this will allow you to actively change the scrolling text as well as the settings of the display. 

Although this project uses the Bluetooth module and 3D printed housings, the only truly required parts are the 8x8 display and an Arduino compatible microcontroller of your choice – in this project, I used a generic ESP8266 board. This project will include all the libraries I used in the code, but I will not be outlining the setup of the ESP8266 board on the Arduino IDE.


===============================================================================================================================
PARTS LIST
===============================================================================================================================
The following parts list contains all the parts I personally used in this project, if you have similar parts that are compatible, they should be interchangeable (like the BT module). The parts I picked are quite inexpensive and readily available. The only parts I wont be mentioning are the inferred parts such as wiring, printer filament… ect

-> ESP8266 Microcontroller – The brains of the project. Can be substituted with any Arduino compatible microcontroller (4$ CAD)
	
-> 8x8 LED Matrix Display – I believe all versions of these displays are similar. I used one with a connected driver chip connected to the underside. Comes in different 	         colors (red, blue, green…ect) mine was specifically named “MAX7219 dot matrix module” (2$ CAD)

-> HC-06 Bluetooth Module – I think other versions of this module would work just the same but this module served me well and was quite cheap. (4$ CAD)

The rest of the parts are more generic. The following list includes most of the other required parts:

	Male-female breadboard cables 
	Female headers
	Protoboard 
	Thing gauge wire (for protoboard)
	Zip ties
	Suction cups (can be found at dollar stores) 


===============================================================================================================================
SOFTWARE
===============================================================================================================================
COMMANDS: (replace Xs with command values)
	…bXX   —>  changes the matrix’s brightness ranging from 0 - 15
	…sXXX  —>  changes the text scroll speed ranging from 0 - 5
	…p     —>  toggles led pulsing for added effect


SETTINGS:
under the “change settings” header starting on line 15, you can change the default values in      the box to allow for different outcomes. Ex: changes default text phrase

NOTE: this is also where you can change the pin connections from the components to the Arduino (what ever type you have)
IMPORTANT^^^


===============================================================================================================================
SETUP 	
===============================================================================================================================
The setup is pretty self-explanatory but I can outline it here real quick. NOTE: detailed photos of the setup can be found in the “photos” folder.

Once the code is adjusted and uploaded to the Arduino, wire the headers and wires as shown in the photos folder (or at least similarly depending on what board you use). If applicable, print the ESP8266 housing and leave the wire (how ever ling you need) from the circuit to the display hanging out of the box. Insert the display into the casing until you snap it in place. Connect the wire to the display then glue the suction cup holder to the back of the casing and slot in the suction cups. 

After applying USB power, test it all work. You’re good to go!


===============================================================================================================================
ANY QUESTIONS, EMAIL: gilbertethan@gmail.com
===============================================================================================================================
