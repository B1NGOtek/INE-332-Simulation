# Truck Management Simulator

An interactive, browser-based discrete-event simulator for exploring truck fleet operations. Configure trucks, loading stations, scales, service-time distributions, travel time, and operating costs, then watch the system evolve and compare performance outcomes.

## Features

- Animated truck, loading, queue, and scale activity
- Configurable fleet size, shift length, station counts, travel time, and costs
- Constant, normal, triangular, and uniform service-time distributions
- Live utilization, waiting-time, throughput, and cost metrics
- Congestion heatmap and event calendar
- Random operational events and optional quiz mode
- CSV export for simulation results
- 24-hour Monte Carlo analysis with a results histogram
- Light and dark themes
- Optional Gemini-powered assistant for changing simulation parameters

## Run locally

No installation or build process is required. Clone the repository and open `index.html` in a modern web browser.

For a local HTTP server, run one of the following commands from the repository directory:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Using the simulator

1. Set the fleet, service-station, loading, scaling, and cost parameters.
2. Select **Run Simulation**.
3. Adjust the playback speed or inspect the live queues and performance metrics.
4. Use the analysis, heatmap, event log, quiz, or CSV export tools as needed.
5. Select **Reset** before starting a fresh scenario.

## Optional AI assistant

The simulator can use the Google Gemini API to interpret natural-language requests and update configuration values. Enter your own Gemini API key in the AI Configuration section to enable it. The key is sent directly from the browser to Google's API and is stored only in that browser's local storage; it is not included in this repository.

The rest of the simulator works without an API key.

## Deployment

This project is a static site and can be deployed directly to Netlify. Use the repository root as the publish directory; no build command is needed.

## Project structure

```text
.
├── index.html             # Complete simulator interface and logic
└── Truck Simulation.html  # Legacy placeholder file
```

## Browser support

Use a current version of Chrome, Edge, Firefox, or Safari. An internet connection is required to load the Google Fonts and Chart.js CDN resources, as well as to use the optional AI assistant.
