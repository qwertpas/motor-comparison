# Motor comparison

Interactive comparison of motor mass, diameter, motor constant and geared power density.

Published at https://qwertpas.github.io/motor-comparison/.

The X axis supports mass and diameter. Diameter consistently uses the nominal diameter encoded in the motor size designation (2306 → 23 mm). The Y axis supports motor constant, power density and P_copper (W). Copper loss uses (motor torque / Km)² with an adjustable motor torque, before gearing, at each source’s stated temperature. Linear extrapolation excludes saturation and other running losses. The TQ ILM family covers all 14 sizes in the 2026 Rev0414 datasheet; rated copper losses are shown separately in motor details. Sources and calculation assumptions accompany each entry.

`index.html` is the self-contained website. `motor-comparison.html` is the same file for offline download. GitHub Pages serves the root of the `main` branch.
