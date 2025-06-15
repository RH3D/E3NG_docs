---
title: Files
layout: default
parent: v1.2S - (standard)
grand_parent: E3NG v1.2
has_children: false
nav_order: 30
permalink: /E3NG_v1_2/standard/files
---
# FILES
{: .text-center }

Before downloading any files, let's take a quick look at the folder and filename structure.

The folder structure is intentionally simple, designed to help you organize parts based on their placement on the printer.

The filenames follow a consistent format based on the part’s position, but pay close attention to the end of each name. Every file includes a small note in brackets, and some may also contain additional information such as size or variant details.

### STANDART FILE NAMING
A typical filename looks like this:
filename_[M_2].stl.
{: .label }
The bracket contains two important pieces of information:

Standard file looks something like this filename**_[M_2]**.stl, where the bracket includes two important informations - first being the part color, second being the quantity of parts required.

color: M = main color, A = accent color, X = part is used only in assembly and is not used on the final printer, use whatever color.
quantity: a number gives you exact amount of printed pieces, X = part either is used or is not. follow the filename and based on other information decide wether you need it or not ( for example "E3" means you only need the part when you build your printer from Ender 3, "E3V2" means you need the part if you start with Ender 3 V2, it also appears on toolhead parts where you need to choose the part based on the probe/hotend/extruder etc. of your choice)

Additional information is only on some parts, is before the brackets and looks like this filename**-S_[A_1]**.stl

size: S = small, M = medium, L = large - this is used for toolhead parts - first choose the hotend mount for the hotend you will use and see the size note in the filename. Then print other parts based on this size. For example Bambulab hotend is toolhead_hotend_bambulab-S_[A-X].stl, so you will print other parts (cooling, probe) with the same "S" size note. If the probe file doesn't have size note, it means it is universal.
printer variant: E3 = Ender 3 used as a base printer, E3V2 = Ender 3 V2 used as a base printer.

{: .warning }
The website is being updated. I apologize for any inconvenience this may have caused. Thank you for your patience and understanding!

continue to:
{: .text-right .lh-0 .pt-8 }

[BUILD GUIDE]{: .btn .fs-6 .fw-300 .text-yellow-300 }
{: .text-right }

[BUILD GUIDE]: https://rh3d.xyz/E3NG_v1_2/standard/build_guide
