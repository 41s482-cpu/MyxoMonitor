# MyxoMonitor

Android/Chrome friendly PWA for ThingSpeak environmental monitoring.

## Features
- ThingSpeak channel defaults to `3561351`
- Field 1 temperature (°C), Field 2 relative humidity (%RH)
- 1h / 6h / 24h / 7d trend views
- 60-second refresh, latest reading, summary statistics, CSV export
- Read API Key is stored only in the browser's localStorage, not embedded in source
- PWA manifest and service worker

## Deploy on Render
Create a Render Static Site connected to this repository/branch.
- Build command: leave empty (or `echo static` if required)
- Publish directory: `.`
- Branch: `main`

Then open the HTTPS URL in Chrome on Android and use menu > Add to Home screen / Install app.

## Data configuration
ESP32 should publish temperature to Field 1 and humidity to Field 2. If the channel is private, enter its Read API Key in the settings screen. If public, leave it blank.
