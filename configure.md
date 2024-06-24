---
title: Printer configuration
layout: default
parent: Into the project
#has_children: true
nav_order: 1
---

# PRINTER CONFIGURATION
{: .text-center }
[CONFIGURATOR DOWNLOAD]{: .btn .fs-6 .lh-0 .fw-300 .text-yellow-300 }
{: .text-center }
_last updated: 2024.06.24 18:00_{: .fs-2 .fw-300 .text-yellow-100 }
{: .text-center }

You will be guided through all the steps you will find in the configurator and you will get helpful and detailed information for all the options to help you with starting your project. This will help explaining differences between the options but all the difference in required parts and materials will be in the configurator.

Configurator is an interactive spreadsheet that will, based on your setup, automatically calculate the right quantities in the Bill of Material, will show you the right parts you need to print and will also show you estimated cost of the BOM and the amount of filament needed. There are two macros included to show/hide the unused parts so with them the chart is much clearer and easy to look through but the macros are not neccessary to run if you have concerns.

It also includes links to buy the parts - all links are affiliate that help with a small amount to the project with no added cost to you.

Recommended options are marked in the setup - those are chosen for good balance between the price and performance.

The configuration is divided into three sections:

[BASE BUILD]

[TOOLHEAD]

[MODS / UPGRADES]

{: .note }
All the pictures bellow are higher resolution, so you can right click - Open image in new tab/window - to view it in more detail.

# BASE BUILD
{: .text-center }

#### BASE PRINTER
Natively supported and tested printers for the conversion. Compatibility with other printers will be verified and tested over time so if you decide to use a different one for the conversion and want to help with the implementation, please give me feedback. There are also dimensions for the aluminium extrusions in the BOM, so you can check the compatibility yourself or even build the printer from scratch.
- Creality Ender 3 - has 2040 x 330 mm extrusion for Y axis - printed spacer is used.
- Creality Ender 3 Pro - default, has 4040 x 350 mm extrusion for Y axis.
- Creality Ender 3 V2 - some have shorter 4040 extrusion for Y axis - printed spacer is used.

![](./assets/images/config/config_base.png)

#### ENCLOSURE
Choosing to enclose the printer or not. V2 style enclosure is better designed and simpler while also adding to the frame rigidity. For the best experience, recommended polycarbonate panels are 4mm thick + 5mm for the front door. Rear electronics cover can be 3mm.

![](./assets/images/config/config_enclosure.png)

#### FRAME
- Printed verticals - legacy version where you don't need to buy extra extrusions. Depending on your filament and market prices, it can also be the cheapest option.
- 2040 update - RECOMMENDED - first stage upgrade with additional alu extrusion. Adds rigidity to the frame.
- Ulti frame - all you need for the best performance, adds two more extrusions to the front, uses butt joints so it requires more driling and tapping threads.

![](./assets/images/config/config_frame.png)

#### Z AXIS RODS
- 2x12 mm rod - legacy version - simple setup that works well enough if your leadscrews are not extremely bent, it also saves few dollars.
- 3x12 mm rod - RECOMMENDED - uses linear rod at the rear leadscrew, makes the bed carriage more stable. This is required if you plan to use tilting bed _(once it is released)_.

![](./assets/images/config/config_z_rod.png)

#### BED CARRIAGE
- Printed - although it works, it is not recommended. It is a backup option for people who cannot use one of the others.
- Stock E3 bed carriage - RECOMMENDED - reuse the stock Ender's bed carriage.
- Metal carriage - cut with laser od water, most rigid option, if you want to get the best out of your printer.
- _Z-tilt bed - in development_

![](./assets/images/config/config_bed_carriage.png)

#### Z WOBBLE COMPENSATION
- None - no Z wobble compensation, T8/8 nuts mounted directly.
- Flexi joint - RECOMMENDED - printed flexible inserts that compensate leadscrew runout.
- WobbleX - more efficient solution by MirageC, but it reduces the max Z by around 22 mm.

![](./assets/images/config/config_bed_wobble.png)

#### Z AXIS DRIVE
- 1 stepper - RECOMMENDED - more foolproof and simple solution with one stepper and long belt driving all 3 leadscrews, also cheaper.
- 3 steppers - for separately driven leadscrews and Z-tilt option. This is required if you plan to use tilting bed _(once it is released)_, but currently this option isn't recommended as there is no compliant mechanism in the bed carriage, which would allow the bed to tilt safely and even a small amount of tilt from improper alignment may increase binding and friction in the Z axis. If you select this option, be very careful and make sure your bed is aligned well resulting in minimal tilt.

![](./assets/images/config/config_steppers.png)

#### LEADSCREW PULLEYS
- Printed - legacy version - cheap and simple option but for good performance it is important to verify that there is no ovality in pulleys and the print is precise.
- Aluminium - RECOMMENDED - precise aluminium pulley equals precise leadscrew rotation.

![](./assets/images/config/config_pulley.png)

#### PSU THICKNESS
- 30 mm - thinner Meanwell PSU used in Ender 3 Pro and in some Ender 3 V2
- 50 mm - thicker PSU used in Ender 3 and in some Ender 3 V2

![](./assets/images/config/config_psu.png)

#### BOARD MOUNT
Currently there are setups for only few motherboards but more will be directly supported in the future. The supported board has DIN rail mount along with cooling fan holder and there is also a FW setup available. But being the boards mounted on DIN rails, it is easy to use any other board. It is also recommended to check the **Optional parts** folder where there are mounts for other electronics commonly used.
- BTT SKR mini E3 v2
- BTT SKR3EZ
- BTT Octopus

![](./assets/images/config/config_board.png)

# TOOLHEAD
{: .text-center }
Toolhead is put together with separate parts for mounting each of the components which makes it super easy to alternate between different type of hardware.

![](./assets/images/config/config_toolhead.png)

#### HOTEND
Select the hotend you want to use, it is generaly recommended to use hotend with higher flow.

![](./assets/images/config/config_hotend.png)

#### EXTRUDER
- Bowden - adapter plate with different bowden connectors - bowden clip / ECAS04 / M6 thread (used on stock Ender extruder) / 1/8' thread (used on stock Ender hotend) / SpiderV3 coupler / Phaetus groove mount adapter
- Original design extruders - adapter plates with the most common mounts to fit the majority of direct drive extruders.
- Integrated - direct drive extruders with integration into the toolhead mount. Makes mounting the extruder more secure and rigid while still being easy to swap.

![](./assets/images/config/config_extruder.png)

#### PART COOLING
- 2 x 4010 - RECOMMENDED - compact and solid option with higher RPM fans - good option for most of the users.
- 2 x 4020 - step up in performance from the previous 4010 fans.
- 2 x 5015 - even more air.
- CPAP - the best choice for extreme cooling and lightweight toolhead, although you can always add auxiliary fans too.

![](./assets/images/config/config_cooling.png)

#### BED PROBE
Choose the right bed probe for you.
- KlickyPCB - RECOMMENDED cheap option with good reliability.
- BDSensor - RECOMMENDED performance option - it is recommended more than Beacon scanner as it doesn't have the "no metal" zone that is forcing Beacon to be further from the nozzle because of the lower LM8LUU. BDSensor is currently more complicated to install but Klipper integration is in the works.

![](./assets/images/config/config_probes.png)

#### ACCESSORIES
- Cable guide - RECOMMENDED for keeping the toolhead wiring clean and safe.
- Breakout board - cheap DIY alternative to toolhead PCB boards using female JST XH connectors and wires directly soldered to them. 5x2pin and 1x3pin
- Accelerometer mount - it is recommended to use nozzle mounted for your accelerometer but this option is easier/faster to use. It has KUSBA as well as ADXL345 mount pattern.

![](./assets/images/config/config_accessories.png)

# MODS / UPGRADES
{: .text-center }

#### STEPPER COOLING
RECOMMENDED - optional active cooling for AB steppers using 4020 axial fans. It is simple yet very effective solution that keeps your steppers cool allowing you to increase the run current and print faster.

![](./assets/images/config/config_AB_cooling.png)

#### FRAME BRACES
Recommended if you are using legacy version of the frame without the enclosure. It adds a bit more rigidity to the frame but other frame variants are rigid enough and the enclosure is even superior in that regard.

![](./assets/images/config/config_brace.png)

#### HANDLES
Handles - RECOMMENDED - to have a good grip on the printer. Handles are automatically added if you select enclosure.

![](./assets/images/config/config_handles.png)

#### LED LIGHTS
- Frame LEDs - RECOMMENDED - LED strips mounted on the frame in the nozzle height to better see the prints.
- Enclosure LEDs - RECOMMENDED - LED strips mounted on the upper edge of the enclosure to light up the inside of the printer.

![](./assets/images/config/config_led.png)

#### AUX COOLING
Auxiliary side cooling using 12032 fans blowing air over the build plate from both sides. For more powerful cooling for your prints.

![](./assets/images/config/config_aux_fan.png)

#### BED WIRING - WAGO 221
For running bed heater cables from your board into the connectors mounted on the bed carriage. It helps with serviceability as you can remove the bed completely without removing all the cables. It uses Wago 221 connectors for the heater wiring and JST XH connectors for the thermistor and/or under bed fan.
- DC BED - for DC - usually 24V bed heaters.
- AC BED - for AC bed heaters including connector for the ground wire.

![](./assets/images/config/config_bed_wiring.png)

#### UNDER BED FAN
RECOMMENDED if you install enclosure. Helps circulating the air inside the chamber and heating it faster and more evenly by sucking the warm air from below the heated bed and blowing it at the bottom. It is moving/mixing air in the entire enclosure.

![](./assets/images/config/config_bed_fan.png)

#### AUTO Z - VORON
Original Voron design for Auto-Z offset with using "Sexbolt" nozzle endstop.

![](./assets/images/config/config_auto_z.png)

continue to:
{: .text-right .lh-0 .pt-8 }

[SOURCING PARTS]{: .btn .fs-6 .fw-300 .text-yellow-300 }
{: .text-right }

[CONFIGURATOR DOWNLOAD]: https://rh3d.github.io/E3NG_docs/configure.html
[BASE BUILD]: https://rh3d.github.io/E3NG_docs/configure.html#base-build
[TOOLHEAD]: https://rh3d.github.io/E3NG_docs/configure.html#toolhead
[MODS / UPGRADES]: https://rh3d.github.io/E3NG_docs/configure.html#mods--upgrades
[SOURCING PARTS]: https://rh3d.github.io/E3NG_docs/sourcing.html
