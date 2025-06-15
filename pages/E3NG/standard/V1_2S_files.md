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
A typical filename looks like this: `filename_[M_2].stl`. The bracket contains two important pieces of information:

#### COLOR
 - `M` = main color
 - `A` = accent color
 - `X` = assembly-use only, part is not used on the final printer, use any color

#### QUANTITY
 - A number indicates how many pieces to print
 - `X` = optional, *you'll need to decide based on your configuration. If you are not sure, it is recommended to view the build guide to become familiar with the part function, for example:*
   - `E3` = needed only for Ender 3 as a base printer, *eg. `frame_bottom_fix_left_E3_[M-X].stl`*
   - `E3V2` = needed only for Ender 3 V2 as a base printer, *eg. `electronics_power_switch_front_E3V2_[M-X].stl`*
   - Also present on toolhead parts.

### OPTIONAL FILE ATTRIBUTES
Some files include additional descriptors before the bracket which help you decide the quantity needed if `X` is specified in the bracket, like this: `filename-S_[A_X].stl`.

#### SIZE
 - `S` = small
 - `M` = medium
 - `L` = large

*This primarily applies to toolhead parts. Choose the hotend mount based on the hotend you’re using, then print the other parts (cooling ducts, probe mounts, etc.) using the same size designation.*

Example: `toolhead_hotend_bambulab-S_[A-X].stl`
  - indicates size `S`.
    - *Use the same size prefix for related parts - `toolhead_fanduct_4010_S_[A-X].stl` and `toolhead_probe_....._S_[A-X].stl`*
  - If a probe file has no size specified, it's considered universal.

#### PRINTER VARIANT
 - `E3` = Creality Ender 3 used as a base printer for conversion.
 - `E3V2` = Creality Ender 3 V2 used as a base printer for conversion.



{: .warning }
The website is being updated. I apologize for any inconvenience this may have caused. Thank you for your patience and understanding!

continue to:
{: .text-right .lh-0 .pt-8 }

[BUILD GUIDE]{: .btn .fs-6 .fw-300 .text-yellow-300 }
{: .text-right }

[BUILD GUIDE]: https://rh3d.xyz/E3NG_v1_2/standard/build_guide
