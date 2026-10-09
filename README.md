# Earthquake Explorer: ArcGIS SDK 5.1 prototype

Replace epicentre-lab.html in your GitHub Pages repository. Serve over HTTPS; internet and WebGL are required. No build step. Not published by the assistant.

## Implemented
ArcGIS 5.1 CDN; arcgis-scene and arcgis-map components; satellite basemap; world elevation; 3D GraphicsLayers and symbols; programmatic SliceAnalysis/SlicePlane; underground navigation and reduced opacity; locator map; surface arrival footprints; underground wavefront wireframes and direct-ray markers; three recording cards in Measure; staged distance constraints and geometric depth solve. Simulated station coordinates now use Valencia, Zagreb, Tripoli and Athens. They are not real seismic monitoring stations.

## Validation status: prototype, not live-verified
JavaScript syntax and offline Chromium controls/solver tests passed, including recovery of the 120 km synthetic depth. A live attempt did not load SDK 5.1 in the execution environment. Basemap/elevation rendering, SliceAnalysis placement, camera framing, locator initialization, station hit testing, animation performance and wave visibility remain UNVERIFIED. Test after hosting before classroom use. Below-ground mode uses both slice and 30% ground opacity, not a true volumetric cutaway. If slice setup fails, transparency is retained. The mathematical Earth is spherical; the geographic renderer uses its own Earth representation.

## Model
One fixed synthetic source: 39 N,10 E,120 km depth. Earth radius 6371 km. P=6 km/s,S=3.5 km/s. Straight chord distance generates arrival times. S-P times 8.4 gives distance to focus. Three sphere equations yield candidate positions; fourth timing selects an interior candidate. Depth=Earth radius minus focus radial distance. Surface rings are intersections of modelled body-wave spheres with the spherical surface, not physical surface waves. No refraction, reflections, core effects, real earthquake feed, uncertainty interval or noisy-data least-squares fit.

## Hosting check
Confirm geographic scene loads, both surface rings are visible at 60 seconds, below-ground button exposes the focus/fronts, locator loads, stations open recordings, and model picks recover 120 km. Keep ArcGIS attribution visible. Service access/licensing and any required authentication must be checked for the intended deployment. No credentials are embedded. No student data is stored.

## Documentation
https://developers.arcgis.com/javascript/latest/get-started/
https://developers.arcgis.com/javascript/latest/references/core/analysis/SliceAnalysis/
https://developers.arcgis.com/javascript/latest/references/core/analysis/SlicePlane/
https://developers.arcgis.com/javascript/latest/sample-code/scene-underground/
