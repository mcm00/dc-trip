# dc-trip

Bilingual (English/Español) interactive itinerary map for a July 3 Washington, DC trip: timed stops from Bethesda, museum highlights, parking options, July 4th closure risk zones, and fallback plans.

**Live site:** https://mcm00.github.io/dc-trip/

## How it works

- `index.html` is a self-contained page: itinerary data, stop cards, and an interactive [Leaflet](https://leafletjs.com/) map (vendored in `vendor/leaflet/`, no CDN required).
- If Leaflet fails to load for any reason, the page falls back to a built-in schematic SVG map with the same stops, parking, and closure zones.
- Deployment: pushes to `main` publish the repository root to GitHub Pages via `.github/workflows/pages.yml`.
