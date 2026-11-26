# God's Eye View — Tactical Geospatial Command Center

An interactive 3D geospatial command center and OSINT (Open-Source Intelligence) simulator inspired by the "God's Eye View" (WorldView) series by Bilawal Sidhu. 

It allows users to scrub through 4D timelines to watch geopolitical, intelligence, and aerospace events unfold in real time on an interactive WebGL globe.

---

## Features

1. **Tactical 3D Globe**: Built with `Globe.gl` and `ThreeJS` for high-performance rendering. Displays custom glowing coordinate pins, animated trajectory arcs, and pulsing signal rings.
2. **Interactive 4D Playback Timeline**: Scrub through time, play/pause, and adjust speed multiplier (1x, 5x, 10x, 25x) to watch scenarios unfold.
3. **3 Pre-Loaded Scenarios**:
   - **Strait of Hormuz Transit**: Track a commercial tanker being intercepted/shadowed by fast-attack IRGCN patrol craft, with a US Navy destroyer escorting and an MQ-9 Reaper drone providing overhead video surveillance.
   - **Eastern Europe GPS Spoofing**: Track civilian aircraft navigating around a high-power active GPS jamming dome, watching their telemetry degrade and their paths divert.
   - **Polar Satellite Launch**: Track a Falcon 9 rocket launch from Cape Canaveral entering polar orbit, complete with Stage 1 boostback and landing on a drone ship in the Atlantic.
4. **Entity Inspector HUD**: Select any aircraft, ship, or rocket on the globe to lock onto its telemetry. Features a real-time updating spec sheet, signal logs, and a **simulated canvas-based FLIR/Thermal sensor feed** that draws wireframe tracking profiles with scanlines.
5. **Tactical Log Alert Ticker**: A live, timestamped log feed that outputs intelligence reports sync'd to the current time of the timeline.
6. **Integrated Audio Synthesis**: Dynamic sound effects using the Web Audio API (can be toggled on/off).

---

## Getting Started

Since this is a **zero-dependency, purely client-side application**, it requires **no compilation, node modules, or build servers**. It runs completely in any modern web browser.

### How to Run

1. Simply open the `index.html` file directly in your browser:
   - Double-click `index.html` in your file explorer.
   - Or open your browser and drag the `index.html` file into the window.
2. Rotate the globe by dragging with your mouse. Zoom in/out with the scroll wheel.
3. Use the **Scenario Dropdown** in the header to switch between events.
4. Use the **Timeline Slider** at the bottom to scrub through the event, or click the **Play** button to watch it run.
5. Click on any green/amber/red indicator dot on the globe to lock your tactical sensors onto it.
