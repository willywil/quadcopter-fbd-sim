# Quadcopter Free-Body Diagram Simulator

Private interactive simulator for GPS and RF antenna angles on a pitching quadcopter relative to a ground station.

## How to review

Open `index.html` directly in Chrome (phone or desktop). No server or install required.

- On phone: download the file and open it in Chrome.
- On Windows/Ubuntu: clone the repo or download the file and open it in Chrome.

Sliders control pitch, horizontal range, and altitude. The free-body diagram, LOS line, and angle readouts update live.

## Current status

This repo currently contains a phone-friendly self-contained HTML/JS side-view free-body diagram with:
- Live pitch, position, and altitude controls
- FG (gravity) vertical reference
- GPS antenna angle vs true vertical
- RF line-of-sight to ground station
- Drone RF boresight and misalignment angles

The fuller version developed in the bot sessions (waypoint editor for 0–20 km paths, altitude trajectory, PX4-style controller, Monte Carlo stress test, min/max angle tables, auto-play, link-check coloring, etc.) was built and delivered as direct HTML downloads but was never committed here. It can be added in a follow-up commit when the files are available on the shared computer.

## Planned / previously requested features

- Click-to-add / drag / delete waypoints on a range-vs-altitude plot (0–20 km)
- Flight along the polyline with continuous angle updates
- PX4 control structure (position → velocity → attitude, real default limits)
- Stress-test mode (Monte Carlo + Markov chain) for worst-case GPS/radio clipping
- Min/max tables and link-margin coloring
- Auto-fit view, scrub slider, force/velocity vectors

Feel free to open issues or PRs for the next revision.
