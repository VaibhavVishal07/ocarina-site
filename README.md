# ocarina-site

The landing page for [Ocarina](https://github.com/VaibhavVishal07/Ocarina-Terminal),
a macOS terminal built for people whose first terminal is this one.

One static page. No build step, no dependencies, no framework — open
`index.html` in a browser and that is the site.

```
index.html      the page: markup and styles in one file
assets/         screenshots of the app, taken from a real build
```

## Why it looks like this

The palette and the typeface are the app's own. Colours are the Ocarina
theme's values, and the page is set in [Geist](https://vercel.com/font),
which is what the app itself is bundled with. The page is dark-only on
purpose: every theme Ocarina ships is dark, so a light landing page would
misrepresent the product.

The hero is the app's empty state — a dot-matrix departures board — which
is where the retro treatment comes from. It is the product's own screen
rather than a style applied on top of it.

## Screenshots

`assets/` holds real captures from a build, resized to 1240px and saved as
JPEG. Replace them in place when the interface changes; the filenames are
referenced directly from `index.html`.

## Serving it

Anything that serves static files will do. For GitHub Pages, enable Pages
on this repository with the source set to the `main` branch, root folder.
