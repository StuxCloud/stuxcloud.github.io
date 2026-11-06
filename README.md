<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.cloud/logo-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.cloud/logo-dark.png"><img src="https://global.media.stux.cloud/logo-dark.png" height="100" alt="Stux.Cloud Logo"></picture>
</p>

# GitHub Pages Redirect

Stux.Cloud's GitHub Pages site. Anyone visiting [stuxcloud.github.io](https://stuxcloud.github.io) is sent straight on to Stux.Cloud's GitHub organization, [github.com/StuxCloud](https://github.com/StuxCloud).

## How it works

[`index.html`](index.html) is a single page with an instant meta refresh and a canonical link, both pointing at `https://github.com/StuxCloud`. `.github/workflows/pages.yml` deploys it to GitHub Pages on every push to `main`.

The organization's other GitHub Pages sites (such as [regionpage.stux.cloud](https://regionpage.stux.cloud) and [status.stux.cloud](https://status.stux.cloud)) have their own custom domains, so they aren't affected by this redirect.

## Changing the target

Edit the URL in both tags in `index.html`:

```html
<meta http-equiv="refresh" content="0; URL=https://github.com/StuxCloud">
<link rel="canonical" href="https://github.com/StuxCloud">
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md), and [CHANGELOG.md](CHANGELOG.md) for release history.

## Versioning

This project uses [Date Versioning](https://datevers.ing): each release is numbered by its UTC release date as `YY.MM.DD` (for example `26.10.23`), with `-1`, `-2`… for later releases the same day. See [CHANGELOG.md](CHANGELOG.md) for what changed in each release.

## License

Copyright (c) 2026 Stux.Group. This project is open source and available for use and modification.

---

*Built & Maintained by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.cloud/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.cloud/icon-dark.png"><img src="https://global.media.stux.cloud/icon-dark.png" height="14" alt="Stux.Cloud" valign="middle"></picture> [Stux.Cloud](https://github.com/StuxCloud), Hosted by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stuxedo.com/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stuxedo.com/icon-dark.png"><img src="https://global.media.stuxedo.com/icon-dark.png" height="14" alt="Stuxedo" valign="middle"></picture> [Stuxedo](https://stuxedo.com).  
Stux.Cloud is a part of the <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.group/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.group/icon-dark.png"><img src="https://global.media.stux.group/icon-dark.png" height="14" alt="Stux.Group" valign="middle"></picture> Stux.Group brand of businesses.*
