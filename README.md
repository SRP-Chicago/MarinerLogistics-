# Mariner Logistics Deck

Interactive pitch deck from the Stream Realty Partners Chicago Tenant Rep team for Mariner Logistics. One static page with no build step: open `index.html`, or host the folder on any static host.

## Presenting

- **Navigate:** arrow keys, Page Up/Down, the space bar, swipe, or click a stop on the route bar. `Home` and `End` jump to the first and last slide.
- **Full screen:** the button at the bottom right.
- **Deep links:** `#cover`, `#team`, `#stream`, `#locations`, `#close`.
- **Interactive bits:** stats count up when a slide opens, team photos spotlight on click, and the Stream map has toggles for Stream offices and Mariner's current sites (hover a dot for its city).
- Below 820px wide, the deck becomes one scrolling page for phones.

## Editing

- **Locations:** fill in the `LOCATIONS` array at the top of the script. Any value left `null` shows "To come". The draft tag hides once any site has data.
- **Mariner brand colors:** the `:root` tokens at the top of the style block. The current navy and signal orange are stand-ins until Mariner's official values are confirmed.
- **Client logos:** the logistics clients are typographic wordmarks for now. To use real logos, add files under `assets/clients/` and swap each `<span class="wm …">` for an `<img>` (see the comment in the markup).
- **Team:** Adrian Boone, Jordan Decker, Phil Geiger. Headshots are in `assets/` (600×750 JPG).
- **Map:** `assets/us-map.js` holds the state outlines (us-atlas, Albers USA) and the projected city points.
