# Build Guide

## Required Components
You will need the following tools and components to build the keyboard (not included in the kit):
- Soldering iron and solder
- Flush side cutters
- No-clean flux
- 5 PCB mount 2u stabilizers
- USB Type C cable
- 1.5mm allen wrentch (black screws, knob screw)
- 1.27mm allen wrentch (silver screws)
## Included Components
| Ref     | Component              | Qty | Notes |
| ---     | ---------              | --- | ----- |
| C1, C2  | 22pF Capacitor         | 2 
| C3, C4  | 0.1uF Capacitor        | 2
| C5      | 4.7uF Capacitor        | 1
| D1-92   | 1n4148 Diode           | 92
| D93, D94| 3.6V Zener Diode       | 2
| FUSE    | 500mA Resettable fuse  | 1
| ISP     | 6 pin header           | 1
| OLED    | 4 pin header           | 1
| USB     | GCT USB4085 USB C port | 1
| POWER   | 3mm LED                | 1
| Capslock| 1.8mm LED              | 1
| R1, R7  | 1.5k Resistor          | 2 
| R8      | 470 Resistor           | 1 
| R2, R5  | 5.1k Resistor          | 2 
| R3, R4  | 75 Resistor            | 2 
| R6      | 10k Resistor           | 1 
| U1      | ATmega32A              | 1
|         | 40 pin IC socket       | 1
| RESET, BOOT | 6mm push button    | 1
| Y1      | 16MHz Crystal          | 1
|         | SH1107 OLED display    | 1
|         | EC11 Rotary encoder    | 1
|         | Knob                   | 1
|         | M2 24mm standoff       | 5   | Upper edge
|         | M2 18mm standoff       | 1   | Middle left
|         | M2 15mm standoff       | 1   | Middle right
|         | M2 13mm standoff       | 5   | Lower edge
|         | M2 6mm screw           | 12  | Bottom
|         | M2 8mm screw           | 12  | Top
|         | Rubber Feet            | 4
|         | Red Herring PCB        | 1
|         | Switch plate           | 1
|         | Plate foam (2mm)       | 1
|         | Case foam (1mm)        | 1
|         | Acrylic case layers    | 7

### USB Port
I like doing the USB port first because I have lots of space to work with.  Heat resistant tape will be useful here to keep the usb port in place.
Solder one of the large legs first and check that the port is flush before soldering the other three legs. \
Solder the smaller pins by applying no-clean flux across the pins, then drag a small amount of solder across the pins until all the holes are filled.

![usbc](https://user-images.githubusercontent.com/800930/144701028-55195723-9e37-4ee0-8cce-97262775312a.jpg)

### Zener Diodes (D93, D94)
**This part has specific orientation** - black line on the diode lines up with the square pad.

![d93-d94](https://user-images.githubusercontent.com/800930/144701106-048eda11-7555-440f-929f-435d162cf98d.jpg)

### Resistors (R1-7)
Orientation does not matter. Solder based on the labeled values.
| Ref    | Value |
| ------ | ----- |
| R1, R7 | 1.5k  |
| R2, R5 | 5.1k  |
| R3, R4 | 75    |
| R6     | 10k   |

![r7-r1](https://user-images.githubusercontent.com/800930/144701127-c6f712bb-3042-41db-84a1-cedace2d651b.jpg)
![r5-r2](https://user-images.githubusercontent.com/800930/144701131-21c64dd1-7633-416c-bf8a-428160addf06.jpg)
![r3-r4](https://user-images.githubusercontent.com/800930/144701132-2d692214-4e4f-490f-b0d4-2cc8aeacc0c6.jpg)
![r6](https://user-images.githubusercontent.com/800930/144701138-a02562c5-93ca-4123-86c0-234244662661.jpg)

### Capslock LED (optional)
Check your switch before doing this.  You may need to solder the LED AFTER you solder you switch.  Short leg \
goes in the square pad.  Use the left holes for a stepped keycap.

![caps-led](https://user-images.githubusercontent.com/800930/144701449-40d33008-8b8e-45d1-aa4d-8b70a19723bb.jpg)

### Capslock 470 resistor (R8)

![r8](https://user-images.githubusercontent.com/800930/144701182-67c8341a-5e76-4710-a43c-32560f133122.jpg)

### Capacitors (C1-4)
Orientation does not matter. Solder based on the labeled values.
| Ref    | Value |
| ------ | ----- |
| C1, C2 | 22uF  |
| C3, C4 | 0.1uF |

![c1](https://user-images.githubusercontent.com/800930/144701002-f5a47306-cd93-4175-97ea-28e250d62aed.jpg)
![c2](https://user-images.githubusercontent.com/800930/144701004-8d5d2d50-50b2-4205-bff3-0730f8d4b878.jpg)
![c3](https://user-images.githubusercontent.com/800930/144701008-4307959c-b4df-4e8c-a564-a3cc2c44e350.jpg)
![c4](https://user-images.githubusercontent.com/800930/144701014-9e5c1946-0949-499e-ae38-582e0e030e89.jpg)

### Capacitor (C5)
**This part has a specific orientation** - longer leg goes in square pad (white mark on the capacitor points up)

![c5](https://user-images.githubusercontent.com/800930/144701035-6b10fdfd-59bd-486b-b245-1fbae8491f38.jpg)

### Fuse
Orientation does not matter. Fold down after soldering.

![fuse](https://user-images.githubusercontent.com/800930/144701037-a6d2cf3c-e2dc-4c4a-9479-6570e64dee23.jpg)

### Crystal (Y1)
Orientation does not matter.

![y1](https://user-images.githubusercontent.com/800930/144701040-a7468eaf-cea2-4d13-ba39-6dadd62de752.jpg)

### Power LED
**This part has a specific orientation** - shorter leg and flat side of the LED line up with the square pad

![power](https://user-images.githubusercontent.com/800930/144701055-2c84b223-0c63-4b7f-9664-c3106bba74f7.jpg)

### Push Button (RESET, BOOT) and IC Socket
Push buttons have no specific orientation. \
Align the notch on the IC Socket with the markings on the PCB. 

![reset-boot](https://user-images.githubusercontent.com/800930/144701061-e5c8209f-8070-471a-a7a6-63bdfa80daea.jpg)
![mcu-socket](https://user-images.githubusercontent.com/800930/144701085-cd923aeb-6c7e-4874-a35e-32b6a685cbe9.jpg)

### Pin Header
Orientation does not matter. 

![isp1](https://user-images.githubusercontent.com/800930/144701062-1a878a6f-ad83-4e97-842a-774bb77d88d0.jpg)

### OLED Header
Orientation does not matter.

![oled-header](https://user-images.githubusercontent.com/800930/144702052-e8cfc8cd-1268-4091-b99a-a7bb67b7605b.jpg)

### ATmega32A
Insert ATmega32A into the IC socket. Make sure the notch on the microcontroller aligns with the notch in the IC socket and the markings on the PCB.

### 1n1418 Diodes (D1-D92)
**This part has a specific orientation** - black line on the diode lines up with the square pad (points up)

![d1-d44](https://user-images.githubusercontent.com/800930/144701156-b7adb07b-b1fe-4656-922f-2ad8b8ffb0b7.jpg)
![d45-d92](https://user-images.githubusercontent.com/800930/144701163-18f6352d-16f1-49ce-b1bf-5cd31e75b652.jpg)

###  Encoder
Install the stabilizers, then place the plate on top. \
Install and solder switches and rotary encoder.

![rotary-encoder](https://user-images.githubusercontent.com/800930/144701095-f28bb927-d644-4fd2-b83b-c39da5a0bfc4.jpg)

## Case Assembly

### Feet #1 - 6mm screws (x5) & 24mm standoffs (x5)

![IMG_3010](https://user-images.githubusercontent.com/800930/144702072-3dcd0fef-d6bb-42ae-84b5-3d1e8edf7058.jpg)

### Feet #2

![IMG_3011](https://user-images.githubusercontent.com/800930/144702075-837352fe-0678-4ef9-91e7-a16be9d48472.jpg)

### Feet #2 - 6mm screw & 18mm standoff

![IMG_3012](https://user-images.githubusercontent.com/800930/144702078-c1acdc79-5fe5-4557-a374-d3e1daf51d71.jpg)

### Feet #4 - 6mm screw & 15mm standoff

![IMG_3013](https://user-images.githubusercontent.com/800930/144702081-bcd66dcb-7b2f-49f9-b565-dbf64f8a94f1.jpg)

### Bottom - 6mm screws (x5) & 13mm standoffs (x5)

![IMG_3014](https://user-images.githubusercontent.com/800930/144702084-7680bce3-54d9-4b60-84f0-760ba9e5e735.jpg)

### Spacer #1

![IMG_3015](https://user-images.githubusercontent.com/800930/144702087-6e7cede8-f8d6-4e22-97cb-9dcbfdbea09b.jpg)

### 1mm Foam

![IMG_3016](https://user-images.githubusercontent.com/800930/144702090-180a1e91-910a-4c2f-9901-e82bb78b438c.jpg)

### Spacer #2

![IMG_3017](https://user-images.githubusercontent.com/800930/144702092-a48e1149-e481-4907-8348-4cbebf39155d.jpg)

### PCB & Switch Plate
Make sure your OLED display has been inserted into the OLED header

![IMG_3018](https://user-images.githubusercontent.com/800930/144702095-edfe0c6c-30a0-40e7-97e6-fff45632605b.jpg)

### PCB top layer

![IMG_3019](https://user-images.githubusercontent.com/800930/144702097-8040aab9-7b8b-45c5-9991-6125a6cbd798.jpg)

### Top layer #1

![IMG_3021](https://user-images.githubusercontent.com/800930/144702099-e8d70c54-8e8f-493c-9f87-66212344c26c.jpg)

### Top layer #2

![IMG_3022](https://user-images.githubusercontent.com/800930/144702101-c941351d-d69b-4a6d-94e6-7f3dbef8ffd2.jpg)

### Clear top: 8mm screws (x12)

![IMG_3023](https://user-images.githubusercontent.com/800930/144702103-6c3f5b47-84c4-4367-88dd-210a8e24e82b.jpg)

### Rotary Knob

![IMG_3025](https://user-images.githubusercontent.com/800930/144702105-8c7c3258-5ced-4c9f-ab02-6bb14084bd6a.jpg)

