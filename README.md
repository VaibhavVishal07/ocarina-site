# ocarina-site

The landing page for [Ocarina](https://github.com/VaibhavVishal07/Ocarina-Terminal),
a macOS terminal built for people whose first terminal is this one.

One static file. No build step, no dependencies, no images — open
`index.html` in a browser and that is the site.

## No screenshots

The interface on the page is not a screenshot of the app; it is rebuilt in
markup. The window is HTML and CSS, and every dot-matrix thing on the page is
generated — painted to a canvas cell by cell. The wordmark comes off the app's
own 5x7 alphabet and the menu bar's card off `ActivityCard`, both copied from
the app rather than drawn again here. They stay sharp at any size, weigh a
fraction of a PNG, and do not go stale the day the interface changes.

The isometric card illustrations are inline SVG for the same reason.

The one figure that is not a piece of the window is the message-to-rows pair
under the task panel: a prompt on the left, the rows it becomes on the right.
The claim there is about a shape — one message going in and three jobs coming
out — and a sentence about a shape is longer than the shape.

## What is drawn

One window, built once and framed on a different part of itself per section —
the tab list, the settings card, the terminal, the task panel and the token
meter, the ⌘K drawer, the error banner and its sheet, and the skills shelf.
The last of those hangs off the window rather than off the terminal pane: it
is 600 points wide in the app, which is wider than the pane, and it is a sheet
over the whole window there too.

The shelf is drawn on its "Start here" tab, which is what it opens on for
somebody who has installed nothing: eight picks led by a line written for the
reader rather than the skill's own description, which is addressed to the agent
that will follow it. Three tabs, and one skeleton under all of them — everything
above them is constant and everything below them is cards.

The menu bar is its own scene, and the only one that is not Ocarina's own
surface. The card is drawn in the app's lamps; everything around it is the
system's, and the window under it is deliberately nobody's — the whole claim of
that section is that the reading you want is the one you want while you are
looking at something else.

**One cell of a departure board.** The seam is the whole idea: a split-flap card
is cut across its middle, and that line has to be visible in every state or it
is a box that fills up. So it is a lit line when the cell is empty and a dark
gap when the cell is full, and row 3 of every grid is the seam.

It is sixteen and a half points square there — square because every other item
in a menu bar is, and a tall narrow one reads as something squeezed rather than
as something drawn to fit — which is too small to study, so the four states are
drawn again beside the copy at four times the pitch. The turning one runs the
same five frames at both sizes: stand, fold through the seam, edge-on, come down
the other side, land. Frames rather than a chase, because a chase is a lamp
brightening and dimming, and a card does not glow, it moves.

It lands on a ring and never on a tick. A tick was the most readable answer in
that slot and the only one that grades the work — an agent stopping means it
stopped talking, not that it managed what you asked, which is why the words say
*back to you* and never *done*.

It is a template image in the app, which the menu bar tints, so it is the one
mark on this page a theme does not reach: white on a dark bar whatever Ocarina
is wearing. The enlarged four take the page's ink for the same reason — a
template has no colour of its own. The line under it in the dropped menu *is*
the theme's, so all nineteen voices are here too.

## Why it looks like this

Colours are the Ocarina theme's own values, and the page is set in
[Geist](https://vercel.com/font), which is what the app itself is bundled
with. It is dark only on purpose: every theme Ocarina ships is dark, so a
light page would misrepresent the product.

The nineteen themes carry their voice as well as their colours — the four
lines a theme writes for working, done, stopped and clear — so the menu the
board drops says what the app would say under the theme you picked.

## Serving it

Anything that serves static files. For GitHub Pages, enable Pages on this
repository with the source set to `main`, root folder.
