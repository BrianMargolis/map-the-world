# map-the-world

A browser tool for calculating the total road mileage within a drawn area. Built to scope out the effort of running every street in a neighborhood.

## Usage

Open `index.html` directly in a browser — no server or build step needed.

1. Use the polygon tool (top-left toolbar) to draw your area on the map
2. Click **Fetch Roads** to load road data from OpenStreetMap
3. Use the road type checkboxes to include/exclude categories
4. Click any individual road segment to exclude/restore it
5. Total mileage updates live as you make changes

## Features

- Draws from OpenStreetMap via the [Overpass API](https://overpass-api.de/)
- Filters by road type (residential, tertiary, service, footway, etc.)
- Per-segment toggling to exclude roads you don't want to count
- Per-type mileage subtotals in the sidebar

## Planned

- Progress tracking (mark roads as completed)
- State persistence (auto-save to browser storage, JSON export/import)

## Dependencies (all CDN, no install needed)

- [Leaflet](https://leafletjs.com/) — map rendering
- [Leaflet.draw](https://github.com/Leaflet/Leaflet.draw) — polygon drawing
- [Turf.js](https://turfjs.org/) — distance calculations
