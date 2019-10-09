# BadUSB-Cable (Evil Crow Cable)
BadUSB cable based on Attiny85 microcontroller (documentation, gerbers, design and schematic).

![EvilCrow](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/Logo1.png)

**Idea:** Joel Serna & Ernesto Sánchez

**Development and implementation:** Joel Serna & Ernesto Sánchez

**PCB design:** Rev0: Jorge Mata, Rev1, Rev2, Rev3, Rev3.1: Ignacio Díaz Álvarez

The developers and collaborators of this project do not earn money with this. 
You can invite me for a coffee to further develop Low-Cost hacking devices. If you don't invite me for a coffee, nothing happens, I will continue developing devices.

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E614OA5)

**We are currently trying to get Evil Crow Cable sold through a distributor. Coming soon...**

**Summary:**
1. History
2. Acknowledgement
3. Electronic components
4. BadUSB Cable without USB connector
	* Rev0 (only for reference)
	* Rev1 (only for reference)
	* Rev2 (final version)
	* Rev3 (final version, this version is easier to weld on a mobile cable)
	* Rev3.1 (final version, Holes D+ and D- removed)
5. Information
	* Rev0 (only for reference)
	* Rev1 (only for reference)
	* Rev2 (This version has a smaller size than Rev3)
	* Rev3 (This version is easier to weld on a mobile cable)
	* Rev3.1 (Holes D+ and D- removed)
	* Import the project
	* Introduction
5. Assembly, bootloader and testing
	* Pinout Rev2
	* Pinout Rev3
	* Pinout Rev3.1
	* Assemble Development Kit
	* Hardware need to burn the bootloader
	* Download bootloader
	* Burning bootloader
	* Basic requirements
	* Installation of Digispark USB Driver (Windows)
	* Installation and update of Micronucleus Windows (not tested)
	* Installation and update of Micronucleus Ubuntu
	* Upload Payloads
	* Payloads
	
	
# History

* Start of the project and first BadUSB cable on breadboard (November 2017):

![BadUSB Cable Breadboard](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/badusb-cable-breadboard.jpg)



* First BadUSB cable with USB connector (December 2017):

![BadUSB Cable with USB connector](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/badusb-cable-usb-1.jpg)

![BadUSB Cable with USB connector](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/badusb-cable-usb-2.jpg)



* Finished proof of concept (January 2018):

![BadUSB Cable final test](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/badusb-cable-final-test.jpg)



* Technical presentation of BadUSB cable and first PCB design (Rev0) presented at Hackplayers Conference (February 2018):

![Design 1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/first-version-1.png)

![Design 1-1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/first-version-2.jpg)



* Rev1 of BadUSB cable design (January 2019):

![Rev1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-1_6*12mm.jpeg)

**NOTE:** More information in Rev1 section.



* Rev2 of BadUSB cable design (May 2019):

![Rev2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-2_6*10mm.png)

**NOTE:** More information in Rev2 section.



* First PCBs (July 2019):

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/first-pcbs-3.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/multi1.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/multi2.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/multi3.jpeg)

* BadUSB Cable Rev2 (August 2019):

![0](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/finalcable0.jpeg)

![1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/finalcable1.jpeg)

![2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/finalcable2.jpeg)

* Rev3 of BadUSB cable design (September 2019):

![Render Rev3](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/render-rev3.png)

* Development kit (September 2019)

![Dev kits](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/dev-kits.jpg)

* BadUSB Cable Rev3 (September 2019)

![Rev3 cable](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/rev3-cable.jpg)

* Development kits and complete cables for Navaja Negra Conference (October 2019)

![NN](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/NN.jpg)

* Rev3.1 of BadUSB Cable design (October 2019)

This version is a solution for Rev3. Rev3 has the holes D- and D+, these holes should NOT be soldered and Rev3 can be confusing.
In Rev3.1 design these holes are eliminated, only VDD and GND are available.
Thanks to @_MG_ for recommending this solution.

![Render Rev3.1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/render-rev31.png)

# Acknowledgement

**PCB design first version:** Jorge Mata & Innovart

	* Jorge Mata: @jor_mata

	* Innovart: @innovart_cc

	* https://innovart.cc

**PCB design final version:** Ignacio Díaz & ForensicSecurity

	* Ignacio Díaz: @Ignacio Díaz Álvarez

	* Forensic & Security: @ForensicSec

	* https://forensic-security.com

# Electronic components

**Rev0:**
* ATTINY85 microcontroller
* 2 x 3.6V zener diode
* 2 x 68 ohm resistor
* 1 x 1.5k resistor

**Rev1-Rev2-Rev3-Rev3.1:**
* ATTINY85 microcontroller (8-soic)
* 1 x 3.6V zener diode common anode (SOT23)
* 2 x 68 ohm resistor (0402)
* 1 x 1.5k resistor (0402)

Electronic components have been bought in: https://www.digikey.com/

# Information

## Rev0
**NOTE:** This Rev0 is included for reference purposes only, Rev2 is the final and full tested version.

![BadUSB Cable Rev0](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/first-version-1.png)

![BadUSB Cable Rev0](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/first-version-2.jpg)

## Rev1
**NOTE:** This Rev1 is included for reference purposes only, Rev2 is the final and full tested version.

![BadUSB Cable Rev1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-1.jpg)

![BadUSB Cable Rev1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-1_6*12mm.jpeg)


## Rev2 (Final version)
Implementation of BadUSB cable based on Attiny85 microcontroller. This version has a smaller size than Rev3-Rev3.1

![BadUSB Cable revision-2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-2_6*10mm.png)

![BadUSB Cable final-1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-3-graph1.png)

![BadUSB Cable final-2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/revision-3-graph2.jpg)

## Rev3 (BadUSB cable version easier to weld)
This version is easier to weld on a mobile cable.

![Rev3](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/rev3-dim.png)

## Rev3.1 (Holes D+ and D- removed)
This version is a solution for Rev3. Rev3 has the holes D- and D+, these holes should NOT be soldered and Rev3 can be confusing.
In Rev3.1 design these holes are eliminated, only VDD and GND are available.
Thanks to @_MG_ for recommending this solution.

![Rev3.1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/rev31-dim.png)

## Import the project
There is a custom built library footprints for this project, remember to import it.

## Introduction
You can order the necessary components with the gerber files in the gerber directory and de BOM (Bill Of Materials).

# Assembly, bootloader and testing
## Pinout Rev2

* **Black:** GND
* **Green:** D+
* **White:** D-
* **Red:** VDD

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/pinout.png)

## Pinout Rev3

* **Black:** GND
* **Green:** D+
* **White:** D-
* **Red:** VDD

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/pinout-rev3-1.jpg)

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/pinout-rev3-2.jpg)

## Pinout Rev3.1

* **Black:** GND
* **Green:** D+
* **White:** D-
* **Red:** VDD

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/pinout-31-1.jpg)

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/pinout-31-2.jpg)

## Assemble development kit

1. Development kit

![Development kit](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/kit.jpg)

2. Add tin on the VDD pin of the USB connector

![Tin USB connector](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/tin-usb-connector-1.jpg)

3. Insert the PCB as shown in the photo

![Insert PCB](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/insert-pcb.jpg)

4. Add more tin on the VDD pin of the USB connector

![Tin USB connector 2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/tin-usb-connector-2.jpg)

5. Add tin on all pins of the USB connector (GND, D+, D- ...)

![Final USB connector](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/final-usb-connector.jpg)

6. Take a mobile phone cable and cut the male USB connector. Then you have to strip the wires as shown in the photo. **NOTE:** STRIP CABLES VDD and GND ONLY!!!

![Strip wires](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/strip-wires.jpg)

7. Add tin to VDD and GND pins.

![Tin VCC GND pin](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/tin-vcc-gnd-pin.jpg)

8. Welding the VDD and GND cables to the VDD and GND pins on the PCB. **NOTE:** Pins D+ and D- are free, you don't have to weld this!!!

![Welding VDD GND](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/Welding-VCC-GND.jpg)

![VCC GND only](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/only.jpg)

9. Add adhesive tape for compact cables and a robust result

![Kit 1](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/kitC-1.jpg)

![Kit 2](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/kitC-2.jpg)

## Hardware needed to burn the bootloader

**NOTE:** If you have a development kit or a complete cable obtained in Navaja Negra Conference... it is not necessary to download and burn the bootloader, continue with the following steps!!!

To burn the bootloader you can use diferent techniques, for the one we use you will need:

* TEST CLIP SOIC 8 (2 X 4)  
* TINY AVR PROGRAMMER 

![clip](https://media.digikey.com/Photos/Pomona%20Photos/5250.JPG)
![programmer](https://media.digikey.com/Photos/Sparkfun%20Elec%20%20Photos/MFG_PGM-11801_sml.jpg)


## Download bootloader

* Download Micronucleus bootloader for ATTINY85: https://github.com/micronucleus

* You can find the bootloader file at micronucleus-t85\firmware\releases folder

* Use "t85_default.hex" for the bootloader

## Burning bootloader

![Bootloader](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/bootloader.jpg)

You must use the correct fuses bit for the bootloader:

* **Extended:** 0xFE
* **High:** 0xDD
* **Low:** 0xE1

AVRISP MKll In System Programmer and AVR Studio software for burning bootloader

![AVRDUDESS](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/avrdudess.png)

## Basic requirements

1. Download Arduino IDE: https://www.arduino.cc/en/Main/Software
2. Install drivers (Windows): https://raw.githubusercontent.com/digistump/DigistumpArduino/master/tools/micronucleus-2.0a4-win.zip
3. Install libusb y UDEV rules (Linux): http://digistump.com/wiki/digispark/tutorials/linuxtroubleshooting
4. Download DigisparkKeyboard library with multiple layout support: https://github.com/ernesto-xload/DigisparkKeyboard
5. Unzip library in Arduino/libraries/directory
6. Edit DigiKeyboard.h file and uncomment #define kbd_es_es
7. Change #define kbd_es_es for your keyboard layout and save the changes
8. Run Arduino IDE
9. Click File and then Preferences
10. Add the JSON URL to the Additional Boards Manager text box: http://digistump.com/package_digistump_index.json
11. Click OK
12. Click Tools > Board > Board Manager
13. Search and Install: Digistump AVR Boards
12. Close the Arduino IDE

## Installation of Digispark USB Driver (Windows)

1. Download Arduino for Digispark which come with USB driver: http://sourceforge.net/projects/digistump/files/
2. Extract the file (DigisparkArduino-Win32-1.0.4-March29.zip) to any folder
3. Execute DigisparkArduino-Win32\DigisparkWindowsDriver\InstallDriver.exe to start installing the USB driver

## Installation and update of Micronucleus Windows (Not tested)

https://github.com/micronucleus/micronucleus

## Installation and update of Micronucleus Ubuntu

1. Create the 49-micronucleus.rules file in the /etc/udev/rules.d/ directory.
2. Copy the contents to the file you just created: https://github.com/micronucleus/micronucleus/wiki/Ubuntu-Linux
3. Reboot the computer or run the following command to update the UDEV rules: udevadm control --reload-rules
4. Download Micronucleus with the following command: git clone https://github.com/micronucleus/micronucleus.git
5. Access the Micronucleus/Commandline directory with the following command: cd micronucleus/commandline
6. Compile with the following command: make
7. Access the Micronucleus/Commandline directory with the following command: cd ~/.arduino15/packages/digistump/tools/micronucleus/2.0a4/
8. Create a backup of Micronucleus with following command: mv micronucleus micronucleus.old
9. Copy the latest version of Micronucleus to this directory with the following command: cp ~/PATH/micronucleus/commandline/micronucleus .
10. Reboot

## Upload Payloads

1. Download payloads: https://github.com/joelsernamoreno/badusb_examples/tree/master/attiny85_digispark
2. Run Arduino IDE
3. Open Payload with Arduino IDE
4. Click tools and select Board: Digispark (Default - 16.5 Mhz)
5. Click Upload
6. Connect the BadUSB cable when the Arduino IDE says to connect it.

**Demo video:** https://twitter.com/JoelSernaMoreno/status/1181296289323130882?s=19

![Sketch](https://github.com/joelsernamoreno/BadUSB-Cable/blob/master/images/upsketch.jpg)

## Payloads

You can get payloads in the following repository:

https://github.com/joelsernamoreno/badusb_examples/tree/master/attiny85_digispark
