# VOID16
*A 4x4 handwired macropad*

![VOID16](https://i.imgur.com/ExFBLPU.jpg)

The VOID16 is a 3d printed, handwired, 4x4 macropad running QMK Firmware on a Pro Micro controller.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is(if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the threads might get stripped.

# Handwiring guide

I've also put together a pretty visual handwiring guide for the VOID9, that you can browse over [here](https://victorlucachi.ro/journal/void9-wiring-guide/).

| ![](https://i.imgur.com/MHTt02w.jpg) 	| ![](https://i.imgur.com/TzdhlCM.jpg) 	| ![](https://i.imgur.com/vTpQaXI.jpg) 	|
|---------------------------------------	|---------------------------------------	|---------------------------------------	|

# Bill Of Materials

* 16 x diodes (tme.eu [link](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/)/aliexpress [link](https://www.aliexpress.com/item/32729204179.html))
* 16 x cherry mx style switches
* 24 AWG (0.2 mm2) wire
* 1 x Pro Micro (aliexpress [link](https://www.aliexpress.com/item/32902569443.html))
* 1 x EC11 Rotary Encoder (optional/aliexpress [link](https://www.aliexpress.com/item/32872039030.html)/mounted to the plate using [this adapter](https://www.thingiverse.com/thing:3770166))
* 4 x M3x10 allen head screws (tme.eu [link](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/)/13mm overall length, 5.5mm diameter head)
* hot glue for securing the pro micro to the bottom case(optional, but recommended)

# Pin assignment

    ROW0    ROW1    ROW2    ROW3
    D3      D2      D1      D0
    
    
    COL0    COL1    COL2    COL3
    E6      D7      C6      D4


    Encoder Pad A           Encoder Pad B
    F5                      F4

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/dev_void/keyboards/handwired/void16). Edit them to suit your own needs and build the firmware following the QMK docs.

If you plan on using the VIA keymap dont forget to download the json definitions file linked in this repository.

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).
