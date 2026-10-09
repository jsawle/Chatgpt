# Earthquake Theatre v1.0
Replace your hosted epicentre-lab.html with the file in this package. Or open it directly in a modern browser. No dependencies or build step.

Complete UI rebuild: large rotatable regional curved-Earth cutaway; P/S wavefronts visible by default; three chapters Watch/Measure/Solve; evidence desk appears only when needed; automatic pauses at station arrivals; numeric and trace picks; staged distance spheres; fourth-station timing; latitude/longitude/depth calculation; schematic globe context; keyboard rotation with arrows and zoom with +/-.

Starts paused at 24 seconds to make waves immediately visible. Restart begins at zero. Watch is a teaching demonstration, not a hidden-source challenge. This version uses one fixed synthetic event at 39 N,10 E,120 km depth. Adjustable scenarios/depth and uncertainty controls from the earlier prototype are not included. Globe context is schematic, without satellite imagery or continents. Geometry is 3D Cartesian, rendered using a custom Canvas projection rather than WebGL. Wireframes and cut faces are explanatory; this is not a photorealistic volumetric renderer.

Model: spherical Earth radius 6371 km; homogeneous P=6 km/s,S=3.5 km/s; straight chord distances; three sphere candidates and fourth distance select the focus. Depth=radius minus radial distance. No refraction, reflections, core effects, noisy-data least-squares fit or confidence interval.

Validation: offline Chromium rendered both wave colours; tested 120 km depth recovery, arrival auto-pause, chapter navigation, mobile width and no JS errors. Browser screenshots inspected. Not tested with students or across all browsers.
