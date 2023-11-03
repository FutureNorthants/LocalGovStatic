---
layout: page
title: Popular links
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

Popular links allows you to display a list of popular links at the top of the homepage or a landing page.

View the [Landing page template](/templates/landing-page/) for an example of popular links.

You can set a list of `popular_links:` in the page's front matter, setting the name and link for each item.

```yaml
layout: landing-page
title: My landing page
popular_links:
  - name: View the reusable components
    link: /components/
  - name: View the default templates
    link: /templates/
  - name: Read about configuration options
    link: /configuration/
```

## Custom title

To override the default 'Popular links' heading, set `popular_links_heading:` in your page's front matter.

```yaml
layout: landing-page
title: My landing page
popular_links_heading: Custom popular links heading
popular_links:
  - name: View the reusable components
    link: /components/
  - name: View the default templates
    link: /templates/
  - name: Read about configuration options
    link: /configuration/
```
