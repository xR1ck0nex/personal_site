# Personal page

My personal website: a short introduction, a write-up of the home server it runs on, my other projects and my background.

It is a static page, served by Nginx from my own Raspberry Pi 5.

## Features

- **No build step.** Plain HTML and CSS plus a few lines of JavaScript for the theme switch; no frameworks or dependencies.
- **No third-party requests.** No external fonts, scripts, analytics or trackers. Fonts come from the visitor's system (a monospace stack for headings, the system sans-serif for text).
- **Light and dark theme** in the [Rosé Pine](https://rosepinetheme.com/) palette (Rosé Pine Dawn for light mode). The page follows the system setting by default; a button switches theme, and the choice is remembered in the browser.
- **Responsive.** The server diagram switches from two columns to one on small screens.
- **Accessible basics.** Semantic sections, labelled diagram and theme button, visible keyboard focus.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page content and the theme switch |
| `style.css` | All styles, including both color palettes |

## Editing

Content lives in `index.html` and styles in `style.css`. Colors are defined as CSS custom properties: the light palette in `:root`, the dark one in the `prefers-color-scheme: dark` block and in `:root[data-theme="dark"]`, so the theme can be changed in one place.
