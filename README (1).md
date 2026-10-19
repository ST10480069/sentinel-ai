# Sentinel AI – Stage 1 (front-end prototype)

All data, camera feeds, detections, locations and notifications are SIMULATED.

## Files (all in ONE folder called `sentinel-ai`)
```
sentinel-ai/
├── index.html   page structure
├── styles.css   colours and layout
├── data.js      sample data
└── app.js       all behaviour
```

## Run it
1. Install VS Code (https://code.visualstudio.com).
2. Open the `sentinel-ai` folder in VS Code (File > Open Folder).
3. Double-click `index.html` to open it in Chrome/Edge/Firefox. (Needs internet for the map.)
   Optional: install the "Live Server" extension, right-click index.html > Open with Live Server.

## Test each feature
- Overview: numbers match the sample data; a red warning lists unmonitored sources.
- Live Monitoring: online / unstable / offline tiles. Offline says "NOT being monitored".
- Settings: set a source to Offline, go back to Live Monitoring and Overview.
- Incident Detection: confidence below the threshold = no incident; above = incident + notifications.
  Running it twice quickly shows duplicate suppression. Offline sources are rejected.
- Incident Reports: filter, open a report, Confirm / Dismiss / Escalate / Resolve. Create a manual incident.
- Map: click markers; red = open incident (registered location only).
- Alerts: simulated delivery; ~20% fail so you can press Retry.
- Activity Log: every action above appears here.
- Settings > Reset restores the sample data.
