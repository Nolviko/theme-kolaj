# Kolaj — a Nolviko theme

A loud, colourful neo-brutalist theme for [Nolviko](https://github.com/Nolviko/nolviko): dotted paper, thick outlines, hard offset shadows and
sticker colours, like a cut-and-paste collage. Light and dark mode, right-to-left scripts, reduced motion and
high-contrast mode are supported.

## Screenshots

| Light mode | Dark mode |
|---|---|
| ![Kolaj home page, light mode](screenshots/home.png) | ![Kolaj home page, dark mode](screenshots/home-dark.png) |

| Thread page | Mobile |
|---|---|
| ![Kolaj thread page](screenshots/thread.png) | <img src="screenshots/mobile.png" width="260" alt="Kolaj on a phone"> |

## Installation

1. Download the latest `nolviko-theme-kolaj-<version>.zip` from this repository's **Releases** page.
2. In your forum: **Admin → Themes → Import**, choose the ZIP and confirm that you trust the package.
3. Build a draft, preview it, then publish. You can switch back to the default theme at any time.

Requires [Nolviko](https://github.com/Nolviko/nolviko) 0.1.0-beta.3 or newer (version 1.0.0 works with 0.1.0-beta.2).

## Development

A theme is a child of the `default` theme: `theme.json` (manifest), `tokens.json` (colours, radius, spacing,
font, density for light and dark mode; contrast is checked on build), `assets/*.css` and template overrides in
`views/`. Only these files go into the ZIP. Every override records the hash of the core template it replaces
(`upstream` in `theme.json`); when core changes that template, the build shows a warning and the theme needs an
update.

## License

[Apache License 2.0](LICENSE), like Nolviko itself.
