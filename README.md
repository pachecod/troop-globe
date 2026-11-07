# U.S. Military Presence Worldwide (3D globe)

An interactive 3D globe showing U.S. troop deployments by country, built with [globe.gl](https://globe.gl).
Search for a country or region, hover or tap a country for its count, and raise countries by troop count.

Adapted from `troopstory/fall2026/globe.html` in [pachecod.github.io](https://github.com/pachecod/pachecod.github.io).

## Files

- `globe.html`: the page and its script
- `globe.css`: styles, including the phone layout (600px wide or less)
- `troops.csv`: troop counts by country
- `earth-texture.jpg`: Earth image

Other images, country shapes, and libraries load from public CDNs.

## Run locally

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765/globe.html.

## Deploy on Render

`render.yaml` is a Render Blueprint for a static site. In the Render dashboard choose **New > Blueprint**,
pick this repository, and apply. Every push to `main` redeploys the site, which serves the globe at its root URL.
