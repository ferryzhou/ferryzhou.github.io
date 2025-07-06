---
title: "Astroprint set bed and extruder temperature for gcode files"
date: 2022-05-08
---

// Copied from dog gcode file come with ender 3 pro package.

add these to beginning

G90
M82
M106 S0
M140 S45
M190 S45
M104 S200 T0
M109 S200 T0

add these to end

M104 S0 ; turn off extruder
M140 S0 ; turn off bed
M84 ; disable motors
G28 X0 Y0
M82 ;absolute extrusion mode
M104 S0
