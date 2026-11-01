# vardoger.eu

The website of [Vardøger](https://github.com/vardoger-eu/vardoger), the digital
twin platform for intelligent mechatronics. One static page, built with
[Zola](https://www.getzola.org); no tracking, no cookies, no external fonts
or CDNs. Two small inline scripts only show the bar at the top once the
page has scrolled; without JavaScript the bar simply stays.

## Build locally

Install Zola (0.19 or newer), then:

```sh
zola serve    # live preview at http://127.0.0.1:1111
zola build    # the site in public/
```

Every text is in `content/_index.md` (front matter `[extra]`); the page is
`templates/index.html`, the styles `static/css/style.css`. A Norwegian
version goes in `content/_index.no.md` with `[languages.no]` in
`config.toml` (see the comment there).

## Deploy

Every push to `main` builds the site and publishes it on GitHub Pages
(`.github/workflows/deploy.yml`) at vardoger.eu.

## Credits

Fonts: Space Grotesk and Inter, under the SIL Open Font License 1.1
(licence texts in `static/fonts`).

All rights reserved.
