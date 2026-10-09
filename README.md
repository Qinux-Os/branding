# Branding

Logos, colours and the rules for using them.

## Assets

| File | Use |
| --- | --- |
| [`svg/qinux-mark.svg`](svg/qinux-mark.svg) | The Q mark. Scales to any size |
| [`svg/qinux-wordmark.svg`](svg/qinux-wordmark.svg) | Mark plus the word "Qinux" |
| [`svg/qinux-mark-mono.svg`](svg/qinux-mark-mono.svg) | Single-colour mark |
| [`colors/palette.json`](colors/palette.json) | Machine-readable colour definitions |
| [`colors/palette.css`](colors/palette.css) | The same colours for the web |
| [`guidelines/USAGE.md`](guidelines/USAGE.md) | How to use the assets correctly |

Raster exports for the desktop, the installer and the web live in
[`logos/`](logos/). They are generated from the SVG sources.

## The mark

The mark is a Q: a ring with a diagonal stroke crossing its lower right, which
is what makes a Q a Q rather than an O. It reads at 16 pixels and at poster
size, and it stays legible in one colour.

The ring is drawn on a 24-unit grid so that it aligns with icon grids and
KDE component sizes.

## Colours

| Name | Value | Use |
| --- | --- | --- |
| Qinux Blue | `#2C6BED` | Primary, accent, selection |
| Qinux Deep | `#163A7A` | Gradients, dark surfaces |
| Qinux Ink | `#0D1117` | Dark backgrounds |
| Qinux Slate | `#4A5568` | Secondary text, borders |
| Qinux Mist | `#E2E8F0` | Light backgrounds, dividers |
| Qinux Paper | `#FFFFFF` | Foreground on dark, light surfaces |
| Accent Amber | `#F59E0B` | Warnings, highlights |

Both themes are defined. Never hard-code a colour outside this palette in
Qinux-facing UI; use the semantic names in
[`colors/palette.css`](colors/palette.css) so light and dark both work.

## Quick rules

The full rules are in [`guidelines/USAGE.md`](guidelines/USAGE.md). The short
version:

1. Leave the mark's clear space equal to the ring's stroke width.
2. Do not stretch, rotate or add effects to the mark.
3. Use the mono version when the background is busy or the size is small.
4. Do not recolour the mark outside this palette.

## Other components

| Repository | Holds |
| --- | --- |
| [`theme`](https://github.com/Qinux-Os/theme) | GTK and Qt styling |
| [`icons`](https://github.com/Qinux-Os/icons) | Icon theme |
| [`wallpapers`](https://github.com/Qinux-Os/wallpapers) | Desktop backgrounds |
| [`sddm-theme`](https://github.com/Qinux-Os/sddm-theme) | Login screen |
| [`plymouth`](https://github.com/Qinux-Os/plymouth) | Boot splash |
| [`fonts`](https://github.com/Qinux-Os/fonts) | Typography |

## Contributing artwork

Artwork proposals belong here; code that renders it belongs in the component
repository. Before proposing a change to the mark itself, read
[`guidelines/USAGE.md`](guidelines/USAGE.md) and open an issue first. The mark
appears in the boot loader, the login screen and the installer, and changing it
is not reversible.

## License

Branding assets are licensed **CC BY 4.0**. You may use and adapt them,
including commercially, with attribution. See [`LICENSE`](LICENSE).

Trademark use is a separate question: you may not imply that Qinux endorses
your product. See the usage guidelines.
