# ocarina-site

The landing page for [Ocarina](https://github.com/VaibhavVishal07/Ocarina-Terminal),
a macOS terminal built for people whose first terminal is this one.

One static file. No build step, no dependencies, no images — open
`index.html` in a browser and that is the site.

## No screenshots

The interface on the page is not a screenshot of the app; it is rebuilt in
markup. The window is HTML and CSS, and every dot-matrix thing on the page is
generated — painted to a canvas cell by cell. The wordmark comes off the app's
own 5x7 alphabet and the menu bar's face off `ActivityFace`, both copied from
the app rather than drawn again here. They stay sharp at any size, weigh a
fraction of a PNG, and do not go stale the day the interface changes.

The isometric card illustrations are inline SVG for the same reason.

## What is drawn

One window, built once and framed on a different part of itself per section —
the tab list, the settings card, the terminal, the task panel and the token
meter, the ⌘K drawer, the error banner and its sheet, and the skills shelf.
The last of those hangs off the window rather than off the terminal pane: it
is 780 points wide in the app, which is wider than the pane, and it is a sheet
over the whole window there too.

The menu bar is its own scene, and the only one that is not Ocarina's own
surface. The face is drawn in the app's lamps; everything around it is the
system's, and the window under it is deliberately nobody's — the whole claim of
that section is that the reading you want is the one you want while you are
looking at something else.

The face is fifteen points square there, which is what the bar gives it and too
small to study, so the four expressions are drawn again beside the copy at six
times the pitch. The working one runs the chase at both sizes: three lamps
along the mouth at the house 72ms a lamp, six dwells to the pass. Only the
mouth moves — eyes that chased as well would read as a face blinking, and a
status item that blinks is asking for something.

It is a template image in the app, which the menu bar tints, so it is the one
mark on this page a theme does not reach: white on a dark bar whatever Ocarina
is wearing, with the chase expressed as alpha rather than as colour. The
enlarged four take the page's ink for the same reason — a template has no
colour of its own. The line under it in the dropped menu *is* the theme's, so
all fourteen voices are here too.

## Why it looks like this

Colours are the Ocarina theme's own values, and the page is set in
[Geist](https://vercel.com/font), which is what the app itself is bundled
with. It is dark only on purpose: every theme Ocarina ships is dark, so a
light page would misrepresent the product.

The fourteen themes carry their voice as well as their colours — the four
lines a theme writes for working, done, stopped and clear — so the menu the
board drops says what the app would say under the theme you picked.

## Serving it

Anything that serves static files. For GitHub Pages, enable Pages on this
repository with the source set to `main`, root folder.
