---
layout: page
title: Configuration
description: How to configure LocalGovStatic
---

The site is built with Jekyll and uses the `_config.yml` for site wide configuration.

## Title

The site's title will display in the top left of the header, unless you have set a logo_url. It will also display in after the page title in every page's meta title tag, which is shown in the browser tab.

```yaml
title: LocalGovStatic
```

## Logo URL

If you would rather display a logo instead of the title in the header, then set the logo_url to point to the image file. SVG files are recommended.

```yaml
logo_url: "/assets/images/path-to-logo.svg"
```

## Copyright

You can set the copyright_name to show as text in the bottom of the footer. Optionally, you can also make the copyright text into a link by setting the copyright_link.

```yaml
copyright_name: Copyright name
copyright_link: "https://www.example.com"
```

## Component Settings

The site wide alert and phase banner are also configured using the `_config.yml` file. Please see the individual pages for notes on how these work.

- [Site Wide Alert](/components/site-wide-alert/)
- [Phase Banner](/components/phase-banner/)

## Jekyll Configuration

For Jekyll configuration, please refer to the official [Jekyll documentation](https://jekyllrb.com/docs/configuration/).
