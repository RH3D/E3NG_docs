---
title: Printing parts
layout: default
parent: Into the project
#has_children: true
nav_order: 3
---

# MATERIAL SELECTION
{: .text-center }

#### ABS/ASA
The most recommended and best choice material for printing parts. It has great properties to withstand increased temperatures, repeated stress and continuous pressure.
<details>
    <summary><h4 style="display:inline-block;margin-left:1.5em;margin-top:0.4em;color:#0096FF"> ABS PRINTING TIPS </h4></summary>
<ol style="margin-left:2em;font-size:14px">
<li>Use enclosure! - the best and the most effective step, even if you use some temporary solution to help eliminating drafts and increasing the ambient air temperature.</li>
<li>Use draft shield - without enclosure, draft shield will help to separate the cold air from the part itself. Draft shield may help even in enclosure when the air temperature is not high enough.</li>
<li>Clean the build plate - no alcohol wiping, use warm water with a dish soap and rub the build plate thoroughly. Wash it well too. Using rough side of the sponge helps.</li>
<li>Clamp your build plate - for magnetic flexible build plates. Your magnet may not be as strong as it used to be and bigger parts can lift the plate corners. Clamp the edges/corners of the build plate to the bed.</li>
<li>Use brim or mouse ears for better adhesion to the build plate.</li>
<li>Less is more - play with the print settings, you may need to decrease the fan speed and print speed.</li>
<li>More is more - try increasing the hotend temperature to properly melt the filament. Try increasing the bed temperature for better sticking parts and hotter environment for the print.</li>
<li>Use ABS+, ASA or a different brand - some filaments are more prone to warping, ASA overall tends to warp less. Do your research or testing to find better filament for you that could warp less.</li>
<li>Use adhesive - if your parts still don't stick to the surface, use some kind of bed adhesive suitable for ABS.</li>
<li>Avoid printing big parts, build the upgraded frame version with 2040 aluminium extrusions, build the "stock E3" or metal bed carriage.</li>
</ol>
</details>

#### PETG
Is significantly more flexible which will reduce stiffness of the frame. It has lower temperature resistance so enclosing the printer will get risky as some of the parts will most likely warp. If you do so, try using bed insulation and print at least the toolhead parts from ABS. It helps if you only print lower temperature materials like PLA and PETG.

#### PLA
Can be used on an open frame printer but not with an enclosure as the parts will definitely warp. The toolhead and bed
carriage should still be printer with higher temperature resistant material.

# PRINTING PARAMETERS
{: .text-center }
All STL files are properly oriented for printing. Some parts include built-in supports, they are marked with ❌.

Depending on your configuration and print settings (brim, draft, purge line), you may need to print bigger parts that require up to 235x235 mm print area. Default print size for Ender 3 is 220x220 mm but you can set it to 235x235 mm in slicer without issues.

#### RECOMMENDED PRINT SETTINGS:
<ul>
<li>4 perimeters</li>
<li>5 top and bottom layers</li>
<li>30% infill</li>
<li>infill type: cubic, gyroid, grid, honeycomb, 3D honeycomb, triangles, stars</li>
<li>0.2 mm layer height</li>
<li>0.45 mm layer width</li>
<li>No supports</li>
</ul>

# CALIBRATION PRINT AND TOLERANCES
{: .text-center }
Before printing parts, it is highly recommended to print the calibration cube. It contains essential features that are related to the project parts like holes for 8mm rods, for LM8LUU bearing, M3 and M5 heat inserts and some other print features to view the print quality.

All the parts are designed with rather tight tolerances (.2mm), so depending on your print quality and precision, it might cause too tight fit mainly on linear rods/bearings. If this is your case, you should clear the holes idealy with a reamer. You can also use properly sized drill bit or even a piece of fine-grit sandpaper on a round stick. Just proceed slowly and carefully so you don’t enlarge the holes too much, the ideal situation is to hand press the parts in with no noticeable play.

Link to download the calibration cube is on the [main site].

# PRINTING PARTS IN COLOR
{: .text-center }
To follow the main/recommended color scheme, look at the PRINTED PARTS list in the CONFIGURATOR – every file is marked with **A** (accent) or **M** (main) color. But this is your printer, be creative and make your own color scheme and design. You can also change the **A/M** values in the table and see how it changes the amount of filament needed.

If you are installing LED lights, there are also diffusers that need to be printed with clean/transparent filament.

continue to:
{: .text-right .lh-0 .pt-8 }

[BUILD INSTRUCTIONS]{: .btn .fs-6 .fw-300 .text-yellow-300 }
{: .text-right }

[main site]: https://rh3d.xyz/into.html
[BUILD INSTRUCTIONS]: https://rh3d.xyz/build_guide.html
