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

You will be guided through all the steps you will find in the configurator and you will get helpful and detailed information for all the options to help you with starting your project. This will help explaining differences between the options but all the difference in required parts and materials will be in the configurator.

Configurator is an interactive spreadsheet that will, based on your setup, calculate the right quantities in the Bill of Material, will show you the right parts you need to print and will also show you estimated cost of the BOM and amount of filament needed.

It also includes links to buy the parts - all links are affiliate that help with a small amount to the project with no added cost to you.

Recommended options are marked in the setup - those are chosen for good balance between the price and performance.

The configuration is divided into three sections:

[BASE BUILD]

[TOOLHEAD]

[MODS / UPGRADES]

# BASE BUILD
{: .text-center }

#### BASE PRINTER
Natively supported and tested printers for the conversion. Compatibility with other printers will be verified and tested over time so if you decide to use a different one for the conversion and want to help with the implementation, please give me feedback. There are also dimensions for the aluminium extrusions in the BOM, so you can check the compatibility yourself or even build the printer from scratch.
- Creality Ender 3 - has 2040 x 330 mm extrusion for Y axis - printed spacer is used.
- Creality Ender 3 Pro - default, has 4040 x 350 mm extrusion for Y axis.
- Creality Ender 3 V2 - some have shorter 4040 extrusion for Y axis - printed spacer is used.

![](./assets/images/config_layout_3.png)

#### ENCLOSURE
Choosing to enclose the printer or not. V2 style enclosure is better designed and simpler while also adding to the frame rigidity. For the best experience, recommended polycarbonate panels are 4mm thick + 5mm for the front door. Rear electronics cover can be 3mm.

![](./assets/images/config_layout_2.png)

#### FRAME
- Printed verticals - legacy version where you don't need to buy extra extrusions. Depending on your filament and market prices, it can also be the cheapest option.
- 2040 update - RECOMMENDED - first stage upgrade with additional alu extrusion. Adds rigidity to the frame.
- Ulti frame - all you need for the best performance, adds two more extrusions to the front, uses butt joints so it requires more driling and tapping threads.

![](./assets/images/config_layout_3.png)

#### Z RODS
- 2x12 mm rod - legacy version - simple setup that works well enough if your leadscrews are not extremely bent, it also saves few dollars.
- 3x12 mm rod - RECOMMENDED - uses linear rod at the rear leadscrew, makes the bed carriage more stable. This is required if you plan to use tilting bed _(once it is released)_.

![](./assets/images/config_layout_2.png)

#### BED CARRIAGE
- Printed - although it works, it is not recommended. It is a backup option for people who cannot use one of the others.
- Stock E3 bed carriage - RECOMMENDED - reuse the stock Ender's bed carriage.
- Lasercut metal - most rigid option, if you want to get the best out of your printer.
- _Z-tilt bed - in development_

![](./assets/images/config_layout_3.png)

#### Z WOBBLE COMPENSATION
- None - no Z wobble compensation, T8/8 nuts mounted directly.
- Flexi joint - RECOMMENDED - printed flexible inserts that compensate leadscrew runout.
- WobbleX - more efficient solution by MirageC, but it reduces the max Z by around 22 mm.

![](./assets/images/config_layout_3.png)

#### Z AXIS DRIVE
- 1 stepper - RECOMMENDED - more foolproof and simple solution, also cheaper.
- 3 steppers - for separately driven leadscrews and Z-tilt option. This is required if you plan to use tilting bed _(once it is released)_, but currently this option isn't recommended as there is no compliant mechanism in the bed carriage, which would allow the bed to tilt safely and even a small amount of tilt from improper alignment may increase binding and friction in the Z axis. If you select this option, be very careful and make sure your bed is aligned well resulting in minimal tilt.

![](./assets/images/config_layout_2.png)

#### LEADSCREW PULLEYS
- Printed - legacy version - cheap and simple option but for good performance it is important to verify that there is no ovality in pulleys and the print is precise.
- Aluminium - RECOMMENDED - precise aluminium pulley equals precise leadscrew rotation.

![](./assets/images/config_layout_2.png)

#### PSU THICKNESS
- 30 mm - thinner Meanwell PSU used in Ender 3 Pro and in some Ender 3 V2
- 50 mm - thicker PSU used in Ender 3 and in some Ender 3 V2

![](./assets/images/config_layout_2.png)

#### BOARD MOUNT
Currently there are setups for only few motherboards but more will be directly supported in the future. The supported board has DIN rail mount along with cooling fan holder and there is also a FW setup available. But being the boards mounted on DIN rails, it is easy to use any other board. It is also recommended to check the **Optional parts** folder where there are mounts for other electronics commonly used.
- BTT SKR mini E3 v2
- BTT SKR3EZ
- BTT Octopus

![](./assets/images/config_layout_3.png)

# TOOLHEAD
{: .text-center }
Toolhead is put together with separate parts for mounting each of the components which makes it super easy to alternate between different type of hardware.

#### HOTEND
Select the hotend you want to use, it is generaly recommended to use hotend with higher flow.

![](./assets/images/config_layout_1.png)

#### EXTRUDER
- Bowden - adapter plate with different bowden connectors - bowden clip / ECAS04 / M6 thread (used on stock Ender extruder) / 1/8' thread (used on stock Ender hotend) / SpiderV3 coupler / Phaetus groove mount adapter
- Original design extruders - adapter plates with the most common mounts to fit the majority of direct drive extruders.
- Integrated - direct drive extruders with integration into the toolhead mount. Makes mounting the extruder more secure and rigid while still being easy to swap.

![](./assets/images/config_layout_2.png)

#### PART COOLING
- 2 x 4010 - RECOMMENDED - compact and solid option with higher RPM fans - good option for most of the users.
- 2 x 4020 - step up in performance from the previous 4010 fans.
- 2 x 5015 - even more air.
- CPAP - the best choice for extreme cooling and lightweight toolhead, although you can always add auxiliary fans too.

![](./assets/images/config_layout_4.png)

#### BED PROBE
Choose the right bed probe for you.
- KlickyPCB - RECOMMENDED cheap option with good reliability.
- BDSensor - RECOMMENDED performance option - it is recommended more than Beacon scanner as it doesn't have the "no metal" zone that is forcing Beacon to be further from the nozzle because of the lower LM8LUU. BDSensor is currently more complicated to install but Klipper integration is in the works.

![](./assets/images/config_layout_1.png)

#### ACCESSORIES
- Cable guide - RECOMMENDED for keeping the toolhead wiring clean and safe.
- Breakout board - cheap DIY alternative to toolhead PCB boards using female JST XH connectors and wires directly soldered to them. 5x2pin and 1x3pin
- Accelerometer mount - it is recommended to use nozzle mounted for your accelerometer but this option is easier/faster to use. It has KUSBA as well as ADXL345 mount pattern.

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
