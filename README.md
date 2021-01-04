# DC5V-2A

![](https://github.com/DL2DW/DC5V-2A/blob/main/Images/DC5V-2A_assembled.jpg)

Sorry for the bad shot, but this thing is too small for my phone camera. :-) 



## DC converter for 5V in TO-3 format

This project came about for two reasons. Firstly, I had dealt with the topic of DC converters and Ripple in general. 

So it was a learning project for me among other things. This model was preceded by some prototypes to achieve an optimal result.

I had set myself the following goals:

- Easy to solder
- As compact as possible
- Avoidance of multilayers
- Low ripple
- Low temperature development under full load
- Inexpensive

The second reason why this project came about: I needed a DC converter that could output 5V (and one with 12V) and 2A. This was needed for another project. 

Of course, I could have bought a ready-made module. But hey, where is the fun and the learning effect? :-)



# Trivia

There was never actually a TO-3 module planned. That had somehow come about in the course of the project. I had already built an extended replica of a Commodore 1541 board. And the linear regulators disturbed me immensely. Not only do they get too hot, they are also hard to get.

By the way, if you have a problem with switching regulators on a Commodore disk drive, at least of the VC1541 series, I recommend to measure the ripple on a living object (the original version with switching regulator) :-)



# Technical

A switching regulator from Texas Instruments in the form of the TPS54332DDAR was used. On the one hand, this is exactly what I needed in terms of data, it is inexpensive and easy to install.

I designed the converter to handle 5V with a continuous load of 2A. At continuous load, it gets a good 50 degrees warm after 2 hours without an additional heat sink. Whereas the outside temperature during the measurement was about 30 degrees.

I have chosen two solderable bolts with internal thread for mounting. If the converter is fixed on a board with a correspondingly large copper surface via these bolts, then the temperature goes down to 38 degrees, at continuous load over several hours.

I could not measure any temperature increase in the nominal range of 1A, where the outside temperature was 30 degrees. 

The DC Converter can easily replace, for example, the well-known 7805 in TO-3 format, but still has enough reserve.

I once created a 3D image, because I unfortunately could not get sharp photos.

![](https://github.com/DL2DW/DC5V-2A/blob/main/Images/DC5V-2A-3D.png)



# BOM

Here is the parts list for the DC converter. Of course you don't have to use exactly these brands. However, I give to note that comparison types, especially if they have a somewhat poorer quality, can have a negative effect on the ripple.

| Quantity | Designator | Manufacturer 1                | Manufacturer  Part Number 1 | Description                                                  |
| -------- | ---------- | ----------------------------- | --------------------------- | ------------------------------------------------------------ |
| 1        | C1         | Murata                        | GRM155R71A104KA01D          | CAP  CER 0.1UF 10V X7R 0402                                  |
| 1        | C2         | Murata                        | GRM32ER61C226ME20L          | Ceramic  capacitor SMD 1210 22 µF 16 V 20 %                  |
| 2        | C3,  C4    | Murata                        | GRM21BR61A226ME44L          | Multilayer  Ceramic Capacitors MLCC - SMD/SMT 0805 22uF 10volts X5R 20% |
| 1        | C5         | Samsung                       | CL21C100JBANNNC             | Cap  Ceramic 10pF 50VDC C0G 5% SMD 0805 Paper T/R            |
| 1        | C6         | Murata                        | GRM033R71A822KA01D          | Multilayer  Ceramic Capacitors MLCC - SMD/SMT 0.0082uF 10volts 10% |
| 1        | C7         | Samsung                       | CL21C122JBFNNNE             | Ceramic  capacitor SMD-0805 1.2nF /50V NP0# J +-5% SAMSUNG , RoHS |
| 2        | CN1,  CN2  | Mill-Max                      | 3125-2-00-80-00-00-08-0     | CONN  PC PIN CIRC 0.040DIA TIN                               |
| 1        | D1         | ON  Semiconductor / Fairchild | SS24FL                      | 40V,  2A SCHOTTKY IN SOD123F                                 |
| 1        | L1         | Eaton  Cooper                 | DR73-4R7-R                  | Ind  Power Shielded Wirewound 4.7uH 20% 100KHz Ferrite 3.09A T/R |
| 1        | R1         | Vishay                        | CRCW0402169KFKED            | VISHAY  - CRCW0402169KFKED - RES, THICK FILM, 169K, 1%, 0.063W, 0402, REEL |
| 1        | R2         | Vishay                        | CRCW040210K2FKED            | VISHAY     CRCW040210K2FKED.      Surface Mount Chip Resistor,  Thick Film, AEC-Q200 CRCW Series, 10.2 kohm, 63 mW, 1%, 50 V |
| 1        | R3         | Vishay                        | CRCW040233K2FKED            | Res  Thick Film 0402 33.2K Ohm 1% 1/16W 100ppm/C Molded SMD Paper T/R |
| 1        | R4         | Vishay                        | CRCW040240K2FKED            | Res  Thick Film 0402 40.2K Ohm 1% 1/16W 100ppm/C Molded SMD SMD Paper T/R |
| 1        | R5         | Vishay                        | CRCW04021K96FKED            | VISHAY     CRCW04021K96FKED       RES, THICK FILM, 1K96, 1%,  0.063W, 0402 |
| 1        | U1         | Texas  Instruments            | TPS54332DDAR                | TEXAS  INSTRUMENTS - TPS54332DDAR - DC/DC CONV, BUCK, 1MHZ, SOIC-8 |





If you liked my project, I would be very happy about a small coffee donation.

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/R6R62T6RN)



# License

The contents of this repository, with the exception of the Docs and Software directories, are released under the following license:

- the "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License" (CC BY-NC-SA 4.0) full text of this license is included in the [LICENSE.CC-NC-BY-SA-4.0](https://github.com/DL2DW/DC5V-2A/blob/main/LICENSE.CC-NC-BY-SA) file and a copy can also be found at https://creativecommons.org/licenses/by-nc-sa/4.0/
