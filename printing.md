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
    <summary><h4 style="display:inline-block;margin-left:1.5em;color:#0096FF;font-weight:bold"> ABS PRINTING TIPS </h4></summary>
<ol>
<li>Use enclosure! - best and most effective, even if you use some temporary solution to help stabilise the printer
surrounding and increase the ambient air around.</li>
<li>Use draft shield - without enclosure, draft shield will help to separate the cold fresh air from the part itself. Draft
shield may help even in enclosure when the air temperature is not as high.</li>
<li>Clean the build plate - my best method is to use the hard side of sponge with warm water and dish soap.</li>
<li>Clamp your build plate - for magnetic flexible build plates. Bigger prints still tend to warp slightly even in enclosure
unless it is really hot. This may lead to lifting corners of the build plate and thus warped parts. Clamp the
edges/corners of the build plate to the bed.</li>
<li>5. Use brim to stick the parts better to the bed.</li>
<li>Less is more - play with the print settings, you may need to decrease the fan speed and/or print speed.</li>
<li>More is more - you may need to increase the hotend temperature to properly melt the filament and get rid of its
internal tension. You may need to increase the bed temperature for better sticking parts and hotter environment
for the print.</li>
<li>Use ABS+, ASA or different brand - some filaments are more prone to warping, ASA overall tends to warp less. Do
your research or testing to find better filament for you that can warp less.</li>
<li>Use adhesive - if your parts still don't stick to the surface, use some kind of bed adhesive suitable for ABS.
Have a look at the mods and alternative parts, there is option to use aluminium extrusions to avoid printing the
rear vertical beams. Also there is a mod for using metal bed carriage plate to avoid printing the big center part and
add stiffness to the bed carriage.</li>
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

# ABS PRINTING TIPS
{: .text-center }
ABS/ASA is the best choice for the build, but it is a material, that is not easy to print on an openframe bedslingers and it
may be very challenging for many users. Here are some print tips:
1. Use enclosure! - best and most effective, even if you use some temporary solution to help stabilise the printer
surrounding and increase the ambient air around.
2. Use draft shield - without enclosure, draft shield will help to separate the cold fresh air from the part itself. Draft
shield may help even in enclosure when the air temperature is not as high.
3. Clean the build plate - my best method is to use the hard side of sponge with warm water and dish soap.
4. Clamp your build plate - for magnetic flexible build plates. Bigger prints still tend to warp slightly even in enclosure
unless it is really hot. This may lead to lifting corners of the build plate and thus warped parts. Clamp the
edges/corners of the build plate to the bed.
5. Use brim to stick the parts better to the bed.
6. Less is more - play with the print settings, you may need to decrease the fan speed and/or print speed.
7. More is more - you may need to increase the hotend temperature to properly melt the filament and get rid of its
internal tension. You may need to increase the bed temperature for better sticking parts and hotter environment
for the print.
8. Use ABS+, ASA or different brand - some filaments are more prone to warping, ASA overall tends to warp less. Do
your research or testing to find better filament for you that can warp less.
9. Use adhesive - if your parts still don't stick to the surface, use some kind of bed adhesive suitable for ABS.
Have a look at the mods and alternative parts, there is option to use aluminium extrusions to avoid printing the
rear vertical beams. Also there is a mod for using metal bed carriage plate to avoid printing the big center part and
add stiffness to the bed carriage.

[main site]: https://rh3d.xyz/into.html
