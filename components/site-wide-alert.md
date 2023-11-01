---
layout: page
title: Site Wide Alert
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

A site wide alert is a banner that can appear at the top of every page on your site, until it is manually dismissed by the user.

You can add a site wide alert by setting the following in your `_config.yml` file.

```yaml
site_wide_alert:
  id: 1
  title: An example alert
  message: This is an example of a site wide alert message with a [link](/components/site-wide-alert/).
```

{% include warning-text.html message="The `id` should be updated for each site wide alert" %}

The id needs to be a unique number to ensure that the new alert will display if the user has previously dismissed a site wide alert with a different id.

The message can contain basic markdown, such as a link.
