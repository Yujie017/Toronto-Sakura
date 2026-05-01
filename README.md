# Toronto Sakura · Cherry Blossom Map

An interactive field map of cherry blossom sites across the City of Toronto. Built to help people find and navigate sakura spots during the short spring bloom window.

**[→ View the map](https://yujie017.github.io/Toronto-Sakura/)** 

---

## What makes this different from a pin map

Instead of dropping a single point per location, each site is outlined as a **polygon viewing zone** — so you can see where the trees actually are and plan how to move through larger parks like High Park or Centennial Park.

## Features

**Bloom status** — Each sakura icon is colour-coded by status for the current season: deep pink for confirmed bloom (from a verified 2026 sighting), light pink for likely in bloom based on the typical peak window, and grey for likely not yet in bloom.

**Bloom forecast timeline** — Each site panel shows a two-week typical peak window derived from ~20 years of records at High Park Nature Centre, adjusted per site and incorporating 2026 sighting data.

**Heads-up alerts** — Sites with construction, closures, or restricted access are flagged with an orange badge in both the map and the site panel.

**All sites list** — Tap ALL in the toolbar to see all 20 sites in one list. Sort A–Z or by nearest after enabling location.

**Site detail panel** — Click any site to see its bloom forecast, 2026 sightings, where-to-see notes, accessibility info, and links to Google Maps and Apple Maps.

**Satellite toggle** — Switch between street map and satellite imagery to scout the terrain before visiting.

**DROP A PIN** — Tap the button in the site panel, or long-press anywhere on the map (right-click on desktop), to copy coordinates and open the spot in any maps app.

**Report a sighting** — Spotted a tree blooming or noticed a closure? Submit via the Report button; sightings are reviewed and added to the map.

## Coverage

20 sites total: 17 from the [City of Toronto's official cherry blossom page](https://www.toronto.ca/explore-enjoy/festivals-events/cherry-blossoms/), plus 3 additional sites confirmed through public photos and on-the-ground sources (Ramsden Park, Toronto Music Garden, Front Campus at U of T).

## How the polygons were made

Each polygon was manually traced to approximate the cherry tree viewing area. Sources used: City of Toronto site descriptions, satellite imagery (Google Maps and Google Earth including historical imagery), Google Street View, and publicly available photos, videos, and articles. Open tree datasets and LiDAR canopy layers were reviewed but not used as primary sources.

## Tech

- [Leaflet](https://leafletjs.com/) for the map
- [OpenStreetMap](https://www.openstreetmap.org/copyright) + [CARTO](https://carto.com/attributions) basemap
- Satellite imagery © [Esri](https://www.esri.com) and partners
- Bloom timing references: [High Park Nature Centre cherry blossom tracker](https://highparknaturecentre.com/cherry-blossom-tracking/)
- Single self-contained HTML file — no build step, no backend

## Deployment

The map is a single `index.html` file with all data embedded. To host it yourself, upload `index.html` to any static hosting service:

- **GitHub Pages** — push to a repo and enable Pages in Settings
- **Netlify** — drag and drop the file at netlify.com
- **Cloudflare Pages** — connect a repo or upload directly

## Disclaimer

Pink shaded areas are approximate outlines, not precise tree locations. Trees may not cover the entire shaded area, and some trees at a site may fall outside it. The bloom forecast is an estimate based on historical records and may not reflect actual conditions in any given year.

## Credits

Data collection, mapping, and design by Yujie Chen. Website built with assistance from AI tools.

Viewing area boundaries and 2026 bloom sightings are both based on publicly available photos, posts, satellite imagery, and community trackers. Many thanks to the Toronto cherry blossom community.
