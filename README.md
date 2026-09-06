# ocarina-site

The landing page for [Ocarina](https://github.com/VaibhavVishal07/Ocarina-Terminal),
a macOS terminal built for people whose first terminal is this one.

One static file. No build step, no dependencies, no images — open
`index.html` in a browser and that is the site.

## No screenshots

The interface on the page is not a screenshot of the app; it is rebuilt in
markup. The window is HTML and CSS, and the dot-matrix wordmark is SVG —
245 circles on a 5x7 grid, the same grid the app draws its departures board
on. It stays sharp at any size, weighs a fraction of a PNG, and does not go
stale the day the interface changes.

The isometric card illustrations are inline SVG for the same reason.

## Why it looks like this

Colours are the Ocarina theme's own values, and the page is set in
[Geist](https://vercel.com/font), which is what the app itself is bundled
with. It is dark only on purpose: every theme Ocarina ships is dark, so a
light page would misrepresent the product.

## Serving it

Anything that serves static files. For GitHub Pages, enable Pages on this
repository with the source set to `main`, root folder.
