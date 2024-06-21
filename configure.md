---
title: Printer configuration
layout: default
parent: Into the project
#has_children: true
nav_order: 1
---

# PRINTER CONFIGURATION
{: .text-center }
[CONFIGURATOR DOWNLOAD]
You will be guided through all the steps you will find in the configurator a you will get helpful and detailed information for all the options to help you with starting your project.

Configurator is an interactive spreadsheet that will based on your setup calculate the right quantities in the Bill of Material, will show you the right parts you need to print but will also show you estimated amount of the BOM cost and filament needed.

It also includes links to buy the parts - all links are affiliate that help with a small amount to the project with no added cost to you.

The configuration is divided into three sections:

[BASE BUILD]

[TOOLHEAD]

[MODS / UPGRADES]

# BASE BUILD
{: .text-center }

#### BASE PRINTER
Natively supported and tested printers for the conversion. Compatibility with other printers will be verified and tested over time so if you decide to use a different one for the conversion and want to help with the implementation, please give me feedback. There are also dimensions for the aluminium extrusions so you can check the compatibility yourself or even build the printer from scratch.
- Creality Ender 3 - has 2040 x 330 mm extrusion for Y axis - printed spacer is used.
- Creality Ender 3 Pro - default setup, has 4040 x 350 mm extrusion for Y axis.
- Creality Ender 3 V2 - similar to E3pro but some have shorter 4040 extrusion for Y axis - use printed spacer to accomodate the length difference.

![](./assets/images/config_layout_3.png)

#### ENCLOSURE
Select if you want your printer to be enclosed or not.

![](./assets/images/config_layout_2.png)

#### FRAME
- Printed
- 2040 update
- ulti frame

![](./assets/images/config_layout_3.png)

#### Z RODS
- 2x12 mm rod
- 3x12 mm rod

![](./assets/images/config_layout_2.png)

#### BED CARRIAGE
- Printed
- Stock E3 bed carriage
- lasercut metal

![](./assets/images/config_layout_3.png)

#### Z WOBBLE COMPENSATION
- None
- Flexi joint
- WobbleX

![](./assets/images/config_layout_3.png)

#### Z AXIS DRIVE
- 1 stepper
- 3 steppers

![](./assets/images/config_layout_2.png)

#### LEADSCREW PULLEYS
- Printed
- Aluminium

![](./assets/images/config_layout_2.png)

#### PSU THICKNESS
- 30 mm
- 50 mm

![](./assets/images/config_layout_2.png)

#### BOARD MOUNT
- BTT SKR
- BTT SKR3EZ
- BTT Octopus

![](./assets/images/config_layout_3.png)

# TOOLHEAD
{: .text-center }

#### HOTEND
Select the hotend you want to use.

![](./assets/images/config_layout_1.png)

#### EXTRUDER
- OEM
- Integrated

![](./assets/images/config_layout_2.png)

#### PART COOLING
- 2x4010
- 2x4020
- 2x5015
- CPAP

![](./assets/images/config_layout_4.png)

#### BED PROBE
Select the right probe for you, FW setup for Klicky or BDSensor

![](./assets/images/config_layout_1.png)

#### ACCESSORIES
- Cables
- Accelerometer
- JST

![](./assets/images/config_layout_4.png)

# MODS / UPGRADES
{: .text-center }

#### STEPPER COOLING
Optional AB stepper cooling

![](./assets/images/config_layout_2.png)

#### FRAME CORNER BRACES
For added frame stabilisation, is good with printed version but is not neccessary

![](./assets/images/config_layout_3.png)

#### HANDLES
Handles - will be automatically added if you select the enclosure

![](./assets/images/config_layout_2.png)

#### LED LIGHTS
- Enclosure
- Frame

![](./assets/images/config_layout_2.png)

#### SIDE COOLING
Aux cooling using 12032 fans, includes spacers for the right height based on your selected hotend.

![](./assets/images/config_layout_2.png)

#### BED HEATER WAGO
For running cables from your board with connectors on the bed carriage, also includes holes for JST XH connectors for thermistor or bed fan.
- AC
- DC

![](./assets/images/config_layout_3.png)

#### UNDER BED FAN
For air circulation and chamber heating

![](./assets/images/config_layout_3.png)

#### SEXBOLT
Original Voron design for Auto-Z offset

![](./assets/images/config_layout_2.png)

---
[CONFIGURATOR DOWNLOAD]: LINK
[BASE BUILD]: https://rh3d.github.io/E3NG_docs/configure.html#base-build
[TOOLHEAD]: https://rh3d.github.io/E3NG_docs/configure.html#toolhead
[MODS / UPGRADES]: https://rh3d.github.io/E3NG_docs/configure.html#mods--upgrades
