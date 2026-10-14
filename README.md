# Mariner Logistics Deck

Interactive pitch deck from Stream Realty Partners' National Tenant Representation team (Adrian Boone and Ryan Boozer) for Mariner Logistics. One static page with no build step: open `index.html`, or host the folder on any static host.

## Presenting

- **Navigate:** arrow keys, Page Up/Down, the space bar, swipe, or click a stop on the route bar. `Home` and `End` jump to the first and last slide; `F` toggles full screen.
- **Opening:** the deck always opens on the cover, even from a link or address that names another slide.
- **Interactive bits:**
  - The cover globe drifts with the pointer.
  - The Stream office map names every office with leader lines, as on Stream's own map; hovering a name or dot highlights it.
  - Stats count up when their slide opens.
  - Soft lime lights blink on the dot grid behind each slide, and thin light trails drift across now and then (off for reduced motion and on phones).
  - On the footprint slide, tap a site (pin, name or list row) to pop out its photo and details; the Stream offices chip adds Stream's Dallas and Fort Worth offices.
  - The thank-you slide has call and email links.
- Below 820px wide, the deck becomes one scrolling page for phones.

## Editing

- **Team:** the `TEAM` array at the top of the script holds names, titles, phones, emails and headshots. It feeds both the team slide and the thank-you slide.
- **Footprint:** the `FOOTPRINT` array (just below `TEAM`) holds Mariner's Coppell, DeSoto and Fort Worth sites: address, square footage, year built, clear height, map position, optional lease terms (DeSoto has them) and an optional `note`. Each site's `photo` points to its building photo in `assets/sites/`, shown in the site's pop-out (set it to `null` to show a placeholder instead). The map is `assets/dfw-map.js` (Dallas–Fort Worth county outlines from us-atlas).
- **Look and feel:** follows marinerlogistics.com: black and navy (`#0D1A2E`) grounds, Mariner lime (`#D3FF28`), off-white type, square corners, and lime hairlines at 20%. The colors are taken from their site stylesheet, and all of them are `:root` tokens at the top of the style block.
- **Type:** Mariner's site uses licensed Adobe/commercial faces (Axia, Video, Trasandina). The deck uses Exo, which their site also loads, plus Chakra Petch in place of Video for labels and buttons.
- **Logos:** `assets/mariner-logo.svg` and `assets/mariner-icon.svg` are the SVGs served on marinerlogistics.com. Client logos live in `assets/clients/` as transparent PNG or SVG files: they show in full color on white tiles. Five were supplied as images; the Hirschbach, loadsmart and ShipBob SVGs come from those companies' websites. Scotlynn is still a typographic wordmark until its file arrives (see the comment in the markup).
- **Photos:** `assets/photos/`, supplied for the deck.
- **Maps:** `assets/us-map.js` holds the US state outlines (us-atlas, Albers USA), the states Stream operates in, and Stream's 21 office points. `assets/dfw-map.js` holds the Dallas–Fort Worth county outlines for the footprint slide.
