# Personal page

My personal website: a short introduction, a write-up of the home server it runs on, my other projects and my background.

It is a single static HTML file, served by Nginx from my own Raspberry Pi 5.

## Features

- **One file, no build step.** HTML and CSS in `index.html`; no JavaScript, no frameworks.
- **No third-party requests.** No external fonts, scripts, analytics or trackers. Fonts come from the visitor's system (a monospace stack for headings, the system sans-serif for text).
- **Light and dark theme** following the visitor's system setting, using the [Rosé Pine](https://rosepinetheme.com/) palette (Rosé Pine Dawn for light mode).
- **Responsive.** The server diagram switches from two columns to one on small screens.
- **Accessible basics.** Semantic sections, labelled diagram, visible keyboard focus.

## Editing
 
All content lives in `index.html`. Colors are defined as CSS custom properties: the light palette in `:root`, the dark one in the `prefers-color-scheme: dark` block and in `:root[data-theme="dark"]`, so the theme can be changed in one place.
 
