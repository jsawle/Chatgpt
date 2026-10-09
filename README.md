# Epicentre Lab v0.5.0
Replace epicentre-lab.html in the existing GitHub Pages repository.

This revision removes explanatory overlays from the globe. The scene, heading, legend and playback now occupy separate layout rows. Duplicate status text is hidden. Surface view is opaque by default; Inside Earth switches to transparency and requests an oblique camera. Focus label is omitted in surface view. View controls remain available in every step. Three original recording cards remain side by side on desktop. The source/depth model is unchanged.

Validation: JavaScript syntax and offline browser checks passed for view controls, progressive navigation, 120 km depth solve, manual picks, challenge, three desktop card layouts and mobile width. Live ArcGIS/WebGL rendering and camera framing were not verified. This revision addresses interface obstruction; it does not replace transparency with a true cutaway or add realistic seismic refraction. No claim of classroom usability validation is made.
