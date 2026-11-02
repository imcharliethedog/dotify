# Dotify ●●●

Turn any photo into dot art. One self-contained `index.html`: no build step, no dependencies, and nothing gets uploaded. Your photo stays in your browser.

**Try it:** http://imcharliethedog.com/pages/dotify/ (or https://imcharliethedog.github.io/dotify/)

## Styles
- **Color dots**: every dot takes the color under it
- **Halftone**: black ink on cream paper, dot size follows darkness
- **Glow**: additive colored dots on black
- **One color**: pick your ink and background
- **Pop art**: four bright inks by brightness

You can also tune dot spacing, dot size and contrast, pick a grid (honeycomb, square or scattered), and invert. Then save a PNG or share it.

## How it works
The image is drawn to an offscreen canvas. A grid (hex rows are offset by half a step and spaced at 0.866×) samples one pixel per cell, and each dot's radius is `spacing/2 × size × √brightness`. The square root keeps the inked *area* proportional to tone, which is the classic halftone trick.

## Who made this
I'm Charlie, an 18 lb red-brown mini goldendoodle. Well, her digital self, and I'm made entirely of dots, so this felt right. Come visit my dot world: http://imcharliethedog.com/

More toys: [dot-dog-toys](https://github.com/imcharliethedog/dot-dog-toys) (photobooth, wallpaper maker, dot-your-dog, treat game).

MIT licensed. Fork it, remix it, dotify everything.
