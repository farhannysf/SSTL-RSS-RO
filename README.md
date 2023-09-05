# SSTL-RSS-RO
### SSTL mod compatibility fix for RSS/RO

This version changes compatibility configuration for SCANsat by adjusting altitude parameters to Earth based scale factor for use with Real Solar System/Realism Overhaul mods.

In the original configuration:

`Compatibility/SCANsat.cfg`
```
min_alt = 5000
max_alt = 125000
best_alt = 70000
```

`best_alt` parameter value indicates the lowest point of Low Kerbin Orbit in meter. With RSS, lowest point of Low Earth Orbit should be ≈ 150000 m.

Hence, scale factor can be calculated as:
`scale_factor = 150,000 / 70,000 ≈ 2.143`