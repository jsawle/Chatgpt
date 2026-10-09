# Epicentre Lab v0.1.0

A single-file ArcGIS 3D classroom prototype matching the dark style of Earth Structure Lab.

## Host on GitHub Pages
Upload `epicentre-lab.html` to the existing Pages-enabled curriculum_artifacts repository. Open that filename under the existing Pages site. No build step or backend is required. Publishing has not been performed here.

## Features
- Four-step learning sequence: arrivals, S-P measurement, circles, location.
- Synthetic seismograms with mouse/touch picks and keyboard-accessible numeric inputs.
- One, two or three station circles, with optional S-P uncertainty bounds.
- Animated P/S travel-distance rings, playback and scrubbing.
- Explore and challenge modes; challenge hides source and travelling rings.
- Three invented Mediterranean scenarios, map-click estimates, teacher notes and sources.

## Scientific scope
All events, stations and waveforms are synthetic. P=6 km/s and S=3.5 km/s are illustrative constant parameters. The model uses spherical great-circle surface distance consistently for arrival times and circles. It ignores depth, refraction and Earth's layered velocity structure. Animated rings are travel-distance analogies, not physical surface waves. This is an epicentre teaching model, not a real earthquake locator. The hypocentre is explained but not rendered or solved. Amplitude is arbitrary.

## Dependencies and privacy
ArcGIS Maps SDK for JavaScript 5.1 is loaded from js.arcgis.com. Satellite basemap requests need internet access and WebGL. No sign-in, telemetry, student-data storage or API key is implemented. External providers receive normal network requests. The app provides timing activities even if the 3D SDK fails.

## Classroom use
Start in Explore and play. Measure P/S, draw circles, then estimate. Use Find it yourself for independent practice. Exact model picks are an explicitly labelled teaching aid. Use one circle to discuss distance versus direction, two for ambiguity, three for agreement. Add uncertainty and critique assumptions.

## Validation
Mathematical consistency and JavaScript syntax were checked during creation. Offline Chromium tests passed for initialization, SDK failure fallback, model picks, station toggles, challenge mode, manual and invalid timing, teacher dialog and mobile horizontal overflow. Live ArcGIS/WebGL rendering was not tested. Full browser/WebGL, school-device, screen-reader and GitHub Pages deployment testing remains necessary. Verify basemap loading, map labels, all scenarios, touch picking, small screens and challenge mode before classroom use.

## Sources
- USGS: The Science of Earthquakes — https://www.usgs.gov/programs/earthquake-hazards/science-earthquakes
- USGS: Earthquake Travel Times — https://www.usgs.gov/programs/earthquake-hazards/earthquake-travel-times
- ArcGIS Scene documentation — https://developers.arcgis.com/javascript/latest/references/map-components/components/arcgis-scene/
