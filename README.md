# Epicentre Lab v0.4.0: clarity update
Replace epicentre-lab.html in the GitHub Pages repository. No build step. Publishing not performed.

UI changes: step-specific controls; plain-language stage titles; Next buttons; explicit Surface / Inside Earth modes; orange diamond focus versus white surface epicentre; separated label offsets; persistent symbol key; current-time explanation; optional expanding wireframes (moving direct-ray markers remain the default); event/answer controls collapsed; three recording cards remain side by side on desktop.

Model unchanged from v0.3: synthetic constant-speed spherical Earth, straight-ray distances, three sphere candidates and fourth timing to select depth. Refraction, depth phases and confidence intervals are not simulated.

Validation: JavaScript syntax and offline Chromium tests passed for progressive controls, view labels, Next navigation, 120 km depth recovery, desktop card visibility at 1280x720/1366x768/1900x900, challenge, manual timing and mobile horizontal width. Live ArcGIS/WebGL rendering and source-label separation have not been validated here. Test hosted version before classroom use.
