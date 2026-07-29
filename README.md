# Vacation Planning

A Jekyll-based static site for planning and documenting vacation itineraries. Published via GitHub Pages at `vivekcg24.github.io/vacation`.

## Project Structure

```
vacation/
├── _config.yaml          # Jekyll site configuration (theme, baseurl, plugins)
├── index.md              # Home page with links to all trip pages
├── README.md             # This file
└── norway2026/           # Norway Cruise August 2026 itinerary
    ├── norwaycruise.md   # Main cruise schedule & port logistics
    ├── eidfjord.md       # Eidfjord port day details
    ├── bergen.md         # Bergen port day details
    ├── kristiansand.md   # Kristiansand port day details
    ├── oslo.md           # Oslo port day details
    └── copenhagen.md     # Copenhagen port day details
```

## Current Trips

- **Norway Cruise August 2026** — 7-night MSC Magnifica cruise from Warnemünde (Berlin) visiting Eidfjord, Bergen, Kristiansand, Oslo, and Copenhagen.

## Adding a New Trip

1. Create a new directory (e.g., `hawaii2027/`).
2. Add markdown files for the trip overview and each destination.
3. Update `index.md` with a link to the new trip.

## Local Development

To preview the site locally:

```bash
bundle exec jekyll serve
```

Then open `http://localhost:4000/vacation/` in your browser.

## Deployment

This site is automatically published to GitHub Pages when changes are pushed to the `main` branch. The `_config.yaml` is configured with:

- **baseurl:** `/vacation`
- **url:** `https://vivekcg24.github.io`
- **theme:** `minima`