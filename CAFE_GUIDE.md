# Gyeonghee Study Cafe Map

An interactive campus-area study cafe guide built with HTML, CSS, JavaScript, and the Tmap Vector JS SDK.

## Features

- Displays six cafe markers around Kyung Hee University.
- Groups cafes into three study-style levels and lets users toggle each group.
- Sorts the list by straight-line distance from the browser's current location (with a campus-gate fallback).
- Shows cafe details and requests a pedestrian route and estimated travel time when a cafe is selected.
- Includes base-map and zoom controls.

## Run locally

1. Open `gyeonghee-cafe-guide.html` from a local web server or an HTTPS page.
2. Register for a Tmap API key and replace both `YOUR_TMAP_APP_KEY` placeholders in the HTML.
3. Configure the key's allowed domains/referrers and usage limits in the Tmap provider settings.
4. Allow location access to sort cafes from your current location. If access is denied, the map uses the campus-gate fallback point.

The map and pedestrian-routing features require a valid Tmap key and network access. Do not commit an active API key to a public repository.
