# WS2812B2020-PB86-XX-Carrier
 Carrier for one or two WS2812B2020 for the PB86-XX switches.

# A brief history
 On 2022-07-27, Adafruit released their new products video on YouTube announcing that they were now carrying the PB86-A1 1P2T switch with LED.  In the first week of August 2022, I stumbled accross this video, amongst others, and was inspired to create this project.

# Background
 This project references PB86-XX switches.  From what I have been able to glean, this is actually a range of switches that appear to come in a number of colors, two different "key top" widths, and from zero to two 3mm LED.  As of writing of this document
 Adafruit was carrying only the PB86-A1 switch.  One of the videos I watched was the JP's Product PICK OF THE WEEK where JP introduces the PB86-A1.  A commentor in the Adafruit discord suggested finding a four lead, 3mm RBG LED that could be used with the switch.
 This is my attempt to push that along.

# Design
 As I am interested in DIY mechanical keyboards, I was interested in having both a version of this switch that was better suited to the 19.05mm spacing of a standard keyboard, and having the maximum flexiability in how many of a particular LED were available
 for flashy animations.  During my research on the PB86-A1 switch, I discovered the wider version of this switch, as well as the fact that it came in zero, one, or two LED variations of both widths, as well as a range of keytop colors.

# Implimentation
 My current design allows for a four pin surface mount header on the bottom of the carrier with +5 (VDD), DI (DIN), DO (DOUT), and GND (VSS) pins, as well as solder pads on the top that allow the mounting of one or two of the WS2812B2020 device.  DOUT of LED 1 is connected
 to DIN of LED 2, and DIN and DOUT of LED 3 are connected to the header on the other side of the PCB.  The intent is to populate only the outer two LEDs, or only the central LED.  Not having any of these switches on hand, I limited the PCB to the foot print of a 0.8mm solder
 pad for a 4 pin header and a wide enough for two 3mm LEDs.  From what I have seen in images, I think this will fit.  3mm LEDs, in my experience, have leads that are not as robust as standard 0.1" (2.54mm) spacing headers, and as such, the switch may require modification to allow
 the thicker leads of a more typical four pin header through the body of the switch.  Also, I was finding it difficult to find both a virtical mount header with leads long enough to pass through the switch as well as one that had only 3mm accross the long axis of the solder pads.  
 This may require custom pins for the leads.
