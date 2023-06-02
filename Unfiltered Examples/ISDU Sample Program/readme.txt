IO-Link Parameter Access on Rockwell Controllers - ISDU Interface on TBEN-L4-8IOL

Author: JGawalt
Date: 7.24.2019

Description: Example program demonstrating the ISDU interface now supported on the TBEN IO-Link masters. 
This simple program demonstrates writing to the standard command parameter of a banner Q4X sensor to turn
the laser on/off as well as reading from the "Measured Value" parameter to view the current position value (0.1mm).

ISDU Message Setup:

	Service Codes (Hex):
		4B - Read
		4C - Write
	Class (Hex):
		67H
	Instance:
		1 for TBEN master 
		     --or--
		slot # for modular I/O
	Attribute:
		Port # 
	Source Elements
		Write: 16 bit index (L.E.), 8 bit subindex (L.E.), Write Data
		Read:  16 bit index (L.E.), 8 bit subindex (L.E.)

