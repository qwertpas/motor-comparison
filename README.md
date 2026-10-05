# Motor comparison

Interactive comparison of motor mass, diameter, motor constant and geared power density.

Published at https://qwertpas.github.io/motor-comparison/.

The X axis supports mass, diameter, nominal envelope volume (cm³) and max no-load speed (rpm). Diameter consistently uses the nominal diameter encoded in the motor size designation (2306 → 23 mm). The Y axis supports motor constant, power density, P_copper (W), nominal envelope volume (cm³) and calculated peak torque (Nm). Copper loss uses (motor torque / Km)² with an adjustable motor torque, before gearing, at each source’s stated temperature. Linear extrapolation excludes saturation and other running losses. The TQ ILM family covers all 14 sizes in the 2026 Rev0414 datasheet; rated copper losses are shown separately in motor details. Sources and calculation assumptions accompany each entry.

`index.html` is the self-contained website. `motor-comparison.html` is the same file for offline download. GitHub Pages serves the root of the `main` branch.

Nominal envelope volume is π × (nominal diameter / 2)² × nominal stack/body length / 1000, with dimensions in mm. Entries lacking a nominal length are omitted whenever either axis uses volume.

The unchecked “Include larger TQ ILM (50 g and up)” checkbox excludes those motors from the plot and axis scaling by default. All entries remain in the catalog table.

Calculated peak torque uses τ ≈ 2πσr²L = 2σV with nominal dimensions. Tangential stress is adjustable from 60–140 kPa (default 70 kPa). With volume in cm³ and stress in kPa, torque in Nm is 0.002 × stress × volume. This geometry estimate is separate from measured and catalog torque ratings.

Max speed uses a positive adjustable voltage (default 24 V) multiplied by the collected Kv in rpm/V, capped at known mechanical limits. TQ values use winding-specific no-load speed / DC-link voltage from manufacturer datasheets. The quoted windings use ideal SVPWM and the existing inferred line-RMS Ke convention. Speed constants, calculation basis and sources appear in motor details. Six entries without speed data are omitted; peak torque versus speed supports 129 entries by default or 141 with larger TQ motors. Peak torque and no-load speed are separate endpoints, not a simultaneous operating point.
