# BetaProtogen

------------------------------------------
Coela Can't! Protogen V1
Document Version: V1.0
------------------------------------------

Included are all of the STL files pre-oriented and ready for printing. But what about the visor? Well, two versions of the vacuum forming buck are included as well so you have the ability to make your own PETG visors. Don't forget that the 3D STEP and IGES CAD files are included, so if the design is not exactly what you want then you have the ability to modify and tweak it!

This design is built around printing on the Prusa i3 MK3s with build dimensions of X:250mm, Y:210mm, and Z:210mm. This design can be printed on smaller printers but may need to be modified or split requiring glue or the addition of screw mounts.

------------------------------------------
ASSEMBLY
------------------------------------------
Parts list:
Generic metric hardware kit (M3, M4, M5): https://www.amazon.com/Assortment-AETTL-Stainless-Assorted-Wrenches/dp/B098ND1GW8/ref=sr_1_4?crid=1XEF2ZF5E4MNY&keywords=metric+hardware+kit+m5&qid=1642454366&sprefix=metric+hardware+kit+m5%2Caps%2C70&sr=8-4
Threaded insert kit (M2, M3, M4, M5): https://www.amazon.com/DYWISHKEY-Knurled-Threaded-Embedment-Assortment/dp/B07MWBJB67/ref=sr_1_2?crid=32CP64EBTXEPU&keywords=metric+threaded+inserts&qid=1642454449&sprefix=metric+threaded+inserts%2Caps%2C65&sr=8-2
M2 Screws: https://www.amazon.com/uxcell-M2x6mm-Thread-Button-Socket/dp/B01B1OD9UQ/ref=sr_1_3?crid=3FN0QLAWPNBSN&keywords=m2x6+screws&qid=1642454542&sprefix=m2x6+screws%2Caps%2C74&sr=8-3

The frame will bolt together with the use of M3 hardware, almost entirely with M3x16mm, ensure the screws are not protruding.
The rear LED board mount will be attached using M2 threaded inserts into the frame and M2x6mm screws for the cover and mount.
The top hinge is mounted with M4 threaded inserts and the hinge mechanism uses an M5 threaded insert and an M5x30mm bolt.
The rear latches are mounted with M3 threaded inserts and M3x10mm screws and use M5x8mm bolts with 20mm M5 grub screws.


------------------------------------------
VISOR
------------------------------------------
Print the V1 or V2 Buck
Make a vacuum former tutorial: https://www.youtube.com/watch?v=Gx66mS7U2vY
Material: Use 0.04" or 1.0mm PETG for proper thickness 

Magnetic mounts visor mount should be attached with a form of adhesive - double sided tape or epoxy - careful with super glue on the visor though! It will cloud it up. Use 6mmx2mm neodymium magnets and check the direction: https://www.amazon.com/FINDMAG-Refrigerator-Magnets-Premium-Whiteboard/dp/B075RZ82HP/ref=sr_1_4?crid=2HQ1A21Y0QQG&keywords=magnet+100+pack+6mm&qid=1645489808&sprefix=magnet+100+pack+6mm%2Caps%2C75&sr=8-4


------------------------------------------
3D Printing
------------------------------------------
Recommended build dimensions: 250mmx210mmx210mm
Resolution: 0.2mm or higher quality
Supports: Not necessary at high resolution, except for jaw.
Brim: Depending on your build surface a brim may be needed to bed adhesion
Material: PETG for frame and PVB for transparent covers - PLA can be used but it can melt if left in hot areas or in vehicles


------------------------------------------
Electronics
------------------------------------------
Controller:
Teensy 4.0: https://www.pjrc.com/store/teensy40.html
OctoWS2811 LED Controller for the Teensy 4.0: https://www.pjrc.com/store/octo28_adaptor.html

Power: 
USB-C Decoy Trigger (USB-C to set voltage out): https://www.amazon.com/Type-C-USB-C-charge-trigger-detector/dp/B07T6LPP9W/ref=sr_1_3?crid=2FWFKCTMHJGR&keywords=usb+c+trigger&qid=1642455379&sprefix=usb+c+trigger%2Caps%2C71&sr=8-3
Buck Converter (5v-38V input to 5V output): https://www.amazon.com/Pololu-Step-Down-Voltage-Regulator-D24V90F5/dp/B01M9C9Q1E
Recommend 20W+ USB-C PD battery

Provide 5V directly to the LED boards from the buck converter and the signal lines from the OctoWS2811 controller.

------------------------------------------
Software
------------------------------------------
Software for controlling the head can be found at: https://github.com/coelacant1/ProtoTracer
To use this, include the ProtoV2Controller.h as the primary controller and pick the animation to display on the face from the animations class. Use the KaiborgV1 animation as a default protogen face.
