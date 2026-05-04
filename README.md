# Toronto Sakura — Field Map

An interactive map of cherry blossom viewing sites across Toronto, with hand-drawn polygon viewing zones, 2026 bloom sightings, and per-site timeline forecasts.

---

## What's on the map

- **Polygon viewing zones** drawn from satellite imagery, street view, and on-the-ground photos — showing exactly where the trees are clustered, not just a pin
- **2026 bloom status** for each site, updated from publicly shared photos and posts
- **Per-site timeline** showing a 2-week forecast window and dated sighting dots
- **Heads-up alerts** for sites with closures, construction, or restricted parking
- **Accessibility info** for each site

## Bloom status icons

| Icon | Status | Meaning |
|------|--------|---------|
| Deep pink flower | Bloom (70%+ open) | Peak bloom, confirmed by a 2026 sighting |
| Light pink flower | Partial bloom | Flowers opening, not yet at peak |
| Flower + green leaf | Late bloom | Winding down, green leaves visible |
| Green leaf | Leaves | Petals mostly gone |
| Grey flower | Buds | Not yet open |
| White flower | No data | No confirmed sighting yet |

## Timeline dot colours

| Colour | Stage |
|--------|-------|
| Dark grey | Bud |
| Light pink | Partial bloom |
| Deep pink | Bloom (70%+ open) |
| Light green | Late bloom |
| Dark green | Leaves |

## How bloom status is determined

1. **Latest observation** in `bloom_2026_observations` takes precedence
2. Manual `bloom_2026` field as fallback
3. Timeline position: before/within the estimated bloom window → No data; after the window → Not in bloom

Bloom stage definitions adapted from [Sakura in High Park](https://www.sakurainhighpark.com/trackers-stages).

## Data sources

- Viewing area boundaries: satellite imagery, street view, community photos
- 2026 sightings: publicly shared Instagram, Reddit, Facebook, and Google Reviews posts
- Bloom timing window: ~20 years of High Park peak bloom records via the [High Park Nature Centre](https://highparknaturecentre.com/cherry-blossom-tracking/), adjusted per site
- Site descriptions: [City of Toronto cherry blossoms page](https://www.toronto.ca/explore-enjoy/festivals-events/cherry-blossoms/)
- Basemap: OpenStreetMap contributors + CARTO; satellite © Esri and partners

## Tech

Single-file HTML — Leaflet.js for the map, embedded GeoJSON, no build step.

## Credits

Data collection, mapping, and design: Yujie Chen. Built with AI assistance.
