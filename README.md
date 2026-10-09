# Epicentre Lab v0.3.0
Upload epicentre-lab.html to replace the existing GitHub Pages file. No build step. Publishing has not been performed.

## New features
Transparent globe; underground focus and surface epicentre joined by a depth line; expanding wireframe P/S fronts in Earth-centred 3D; moving direct-ray markers; adjustable synthetic depth 20-600 km; station distance spheres; location and depth solver; East Point fourth timing reference to distinguish the two three-sphere candidates. The three original traces remain visible side by side on tested desktop sizes. The fourth observation is a numeric S-P gap, not a fourth seismogram.

## Try it
1. Explore: play or scrub waves; use See through the globe and Oblique view.
2. Change source depth; synthetic arrivals recalculate.
3. Use model picks, then step 3 to display distance spheres.
4. Calculate focus. Compare latitude, longitude and depth with Reveal.
5. Clear East Point timing and calculate to demonstrate candidate ambiguity where present.

## Model and limitations
All observations are synthetic. P=6 km/s and S=3.5 km/s in a homogeneous spherical Earth of radius 6371 km. Straight Cartesian chord distance to the focus generates the arrivals. S-P gap times 8.4 gives the sphere radius. Three sphere equations give two candidates; fourth timing and a 0-700 km interior range select the candidate. Depth is Earth radius minus focus radial distance. This is a geometric teaching solver, not a real noisy-data least-squares seismic locator. No confidence interval is calculated. The uncertainty slider bounds station distances only. Refraction, reflection, depth phases, core effects and attenuation are omitted. Wavefront parts outside Earth are mathematical extensions, not waves in air. The geographic rendering uses the SDK globe; the mathematical model is spherical.

## Validation
JavaScript syntax and offline Chromium interaction tests passed. Exact synthetic picks recovered depths 20,120,300,600 km in each of three scenarios (12 combinations). Three cards fit at 1280x720,1366x768,1900x900. Live ArcGIS SDK/WebGL rendering, underground visibility and animation performance have NOT been validated here. Test after hosting before classroom use.

## Science sources
USGS: Determining the Depth of an Earthquake
https://www.usgs.gov/programs/earthquake-hazards/determining-depth-earthquake
USGS: The effect of S-wave arrival times on the accuracy of hypocenter estimation
https://www.usgs.gov/publications/effect-s-wave-arrival-times-accuracy-hypocenter-estimation
ArcGIS: Underground navigation in global mode
https://developers.arcgis.com/javascript/latest/sample-code/scene-underground/
