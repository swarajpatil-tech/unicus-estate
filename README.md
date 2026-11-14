# Unicus Estate — concept site

Live: **https://swarajpatil-tech.github.io/unicus-estate/**

A concept website for Unicus Estate, an 18-acre, 101-plot NA hill project in Igatpuri, about 90 minutes from Nashik. Built as a pitch: the project's Instagram bio pointed at a domain that never loaded.

## What's inside

| File | What it is |
|---|---|
| `index.html` | The whole site. ~84 KB, all CSS and JS inline, no build step. |
| `plan.svg` | The masterplan as inline-ready SVG. |
| `pages.json` | Per-plot data (number, area, status). |
| `assets/` | Photography used across the sections. |
| `social-post/` | Instagram cover and a feed preview for the launch post. |
| `.nojekyll` | So GitHub Pages serves the folder as-is. |

## Editing it

- **Colours and type** live in the `:root` custom properties at the top of `index.html`.
- **Plots** are 101 `<polygon>` elements in the inline SVG, each with `data-status="available|reserved|sold"`. Marking one sold is a one-attribute change; the map, the counter and the legend all read from it.
- **Enquiry number** is in the WhatsApp handler near the bottom of the file.

## Hosting

Static only, so any host works. On GitHub Pages: Settings → Pages → deploy from `main`, root folder. No secrets, no backend, no dependencies.

## Before it goes to a client

The photos in `assets/` are stock stand-ins. Swap in the developer's own photographs first.
