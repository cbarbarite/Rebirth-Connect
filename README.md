# Rebirth Connect (free web prototype)

A personal, mobile-friendly prospect finder for Rebirth Recovery Center. Searches named organizations in OpenStreetMap within about 15 km of a selected city in NJ, NY, or PA using Nominatim and Overpass. Results are not verified clinical referral sources. LinkedIn is a search link only, not profile matching.

## Publish from an iPhone

1. Create a free GitHub account and a new **public** repository, for example `rebirth-connect-app`. A public repository means **all uploaded source files are public**; do not upload private data, passwords, or patient information.
2. Upload `index.html`, `app.js`, `manifest.webmanifest`, and `sw.js` from this ZIP to the repository root using GitHub's web interface (may be easier with Safari's Request Desktop Website).
3. In repository Settings → Pages, choose Deploy from a branch, main, root. Wait for the site URL to appear.
4. Open that HTTPS URL in Safari → Share → Add to Home Screen.

## What works

- Search public OSM data around a city, one category at a time.
- Show map pins, public websites, phones (when available), Google Maps directions, LinkedIn search links.
- Save prospects and private notes locally on the iPhone, and export saved records to CSV.

## Important limitations

- Internet is required for discovery and map tiles. Free OSM endpoints are community services with usage limits and occasional outages. Do not automate bulk three-state scans through public endpoints.
- This is a **manual city-by-city search**; it does not yet scan all three states automatically or find verified decision makers.
- Saved data is in browser localStorage on that device, not backed up, synced, or protected by an app login. Clearing Safari website data may delete it. Export CSV regularly.
- Do not store patient data or PHI. This is not a HIPAA-compliant patient system.
- Free public hosting exposes the app's code, but not browser-local saved prospects. It is not a secure private deployment. For a true private single-user app, add authentication and a suitable backend.
- Overpass query availability, tag quality, and category coverage vary.
