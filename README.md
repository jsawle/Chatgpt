# Epicentre Lab v0.2.0
Replace epicentre-lab.html in your GitHub Pages repository with the supplied file. No build step. Publishing is not performed here.

## Changes
- New workspace layout: compact left controls, unobstructed globe, three recording cards side by side beneath it.
- All three recordings visible without scrolling on desktop layouts at 1366x768 and larger. Controls may scroll on short screens; mobile stacks the cards for readable traces.
- Fictional station names West Ridge, North Peak and South Shore, matching the globe labels. Coordinates are unchanged from v0.1.0. These are not real monitoring stations.
- Circle checkboxes moved into the corresponding recording cards.
- Compact playback within the map; teacher notes in a dialog.

## Model
All events, traces and arrivals are synthetic. Constant illustrative speeds P=6 km/s and S=3.5 km/s; spherical great-circle surface distance. Depth and refraction omitted. Animated rings are travel-distance analogies, not physical surface waves. The S-P uncertainty slider applies to the measured gap. No student data is stored.

## Validation
Offline Chromium checks passed: all three cards visible without scrolling at 1280x720, 1366x768 and 1900x900; syntax, model picks, circle toggles, challenge mode, input validation, teacher notes and mobile horizontal width. Live ArcGIS SDK and WebGL rendering require testing after hosting. External internet requests to the ArcGIS SDK and satellite basemap are required.
