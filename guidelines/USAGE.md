# Brand usage

How to use the Qinux assets correctly.

## The mark

The mark is a ring with a diagonal tail crossing its lower right. The tail is
what makes it a Q. Keep it: do not draw a plain circle.

## Clear space

Leave clear space on all four sides equal to the ring's stroke width, which is
2 units on the 24-unit grid.

```text
      ┌─────────────────────┐
      │   ┌─────────────┐   │  ← 2 units on every side
      │   │             │   │
      │   │     Q       │   │
      │   │             │   │
      │   └─────────────┘   │
      └─────────────────────┘
```

If another element must come closer, shrink the mark rather than removing the
clear space.

## Minimum size

| Variant | Minimum width |
| --- | --- |
| Colour mark | 16px |
| Mono mark | 16px |
| Wordmark | 96px |

Below 16px the tail becomes ambiguous and the mark reads as an O. At that size
use the mono version, which has higher contrast.

## Do not

- Stretch, squash or rotate the mark.
- Change its colours to anything outside the palette.
- Add a shadow, glow, bevel or outline.
- Place the colour mark on a busy or mid-tone background. Use the mono version,
  or put it on a solid surface.
- Rebuild the mark from the shape. Use the SVG.

## Do

- Use the SVG wherever the environment supports it.
- Provide a raster fallback for contexts that cannot render SVG.
- Use the mono version when the background is a photograph or a wallpaper.
- Keep the mark's aspect ratio at 1:1. It is never wider than it is tall.

## Colour

The palette is in [`../colors/palette.json`](../colors/palette.json) and
[`../colors/palette.css`](../colors/palette.css).

Prefer the semantic names in the CSS over literal hex values, so that both
themes work without a second stylesheet.

Qinux Blue on Qinux Ink is 4.6:1, which passes WCAG AA for body text. On
Qinux Paper it does not; use Qinux Deep for text on light surfaces. This is why
`--accent` differs between the two themes in the CSS.

## Typography

Qinux does not ship a brand typeface. The wordmark is set in a generic sans
serif with fallbacks, so it renders predictably everywhere.

In documentation and UI, use the font stack from the
[`fonts`](https://github.com/Qinux-Os/fonts) repository. Do not introduce a
second family for headings only.

## The name

- "Qinux" — capital Q, everything else lowercase.
- Never "QINUX", "qinux" as a sentence start in running text, or "QInux".
- It is a distribution name, not an acronym. Do not expand it.

## Trademark

The assets are **CC BY 4.0**: use them freely, including commercially, with
attribution. See [`../LICENSE`](../LICENSE).

Trademark is a separate question. You may not use the mark in a way that
suggests Qinux endorses your product, your distribution or your service. If you
are building something based on Qinux, say so plainly and do not present it as
Qinux itself.

## Attribution

When the licence requires attribution, a good form is:

```text
Qinux and the Qinux logo are trademarks of the Qinux project.
Licensed under CC BY 4.0. https://github.com/Qinux-Os/branding
```

## Requesting a change

Open an issue before designing anything.

The mark appears in the bootloader, the login screen, the installer, the
wallpapers and the website. A change to it touches all of them, so it needs
agreement before any work starts. A change to a colour token is much cheaper
and often achieves what you actually wanted.
