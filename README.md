# Sigma Protogen

------------------------------------------
Coela Can't! Sigma Protogen
------------------------------------------

Included are all of the STL files pre-oriented and ready for printing. But what about the visor? Well, two versions of the vacuum forming buck are included as well so you have the ability to make your own PETG visors. Don't forget that the 3D STEP and IGES CAD files are included, so if the design is not exactly what you want then you have the ability to modify and tweak it!

This design is built around printing on the BambuLab P1P/P1S/X1C with build dimensions of X:250mm, Y:250mm, and Z:250mm. This design can be printed on smaller printers but may need to be modified or split requiring glue or the addition of screw mounts.

------------------------------------------
ASSEMBLY
------------------------------------------
Parts list:
M3 Screws: M3x12
M2 Screws (if mounting the WS35 panels)
6.25mm / 1/4" Diameter x 6mm / 1/4" depth neodymium magnets (N52): https://www.kjmagnetics.com/proddetail.asp?prod=D44-N52
40mm Fan x 10mm thick recommended

The frame will bolt together with the use of M3 hardware, almost entirely with M3x12mm, ensure the screws are not protruding.

------------------------------------------
VISOR
------------------------------------------
Print the Buck
Make a vacuum former tutorial: https://www.youtube.com/watch?v=Gx66mS7U2vY
Material: Use 0.06" or 2.0mm PETG for proper thickness 

Magnetic mounts visor mount should be attached with a form of adhesive - double sided tape or epoxy - careful with super glue on the visor though! It will cloud it up. Use 6mmx2mm neodymium magnets and check the direction: https://www.amazon.com/FINDMAG-Refrigerator-Magnets-Premium-Whiteboard/dp/B075RZ82HP/ref=sr_1_4?crid=2HQ1A21Y0QQG&keywords=magnet+100+pack+6mm&qid=1645489808&sprefix=magnet+100+pack+6mm%2Caps%2C75&sr=8-4


------------------------------------------
3D Printing
------------------------------------------
Recommended build dimensions: 250mmx250mmx250mm
Resolution: 0.2mm or higher quality
Supports: Not necessary at high resolution, except for jaw.
Brim: Depending on your build surface a brim may be needed to bed adhesion
Material: TPU 98A/95A for the frame or PETG. PLA is not recommended (it will melt in hot weather)


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
