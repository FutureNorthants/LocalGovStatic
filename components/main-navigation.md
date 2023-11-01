---
layout: page
title: Main navigation
related: navigation_related
breadcrumbs:
  - name: Components
    link: /components/
---

To add links to the main navigation menu, create a `navigation.yml` file in the `_data` directory and add links using the following format:

```yaml
items:
  - name: Components
    link: /components/
  - name: Templates
    link: /templates/
  - name: News
    link: /news/
```

## Dropdown menu

To add links to a dropdown menu, add a `dropdown:` property, setting the name and link for each item.

```yaml
items:
  - name: Templates
    link: /templates/
    dropdown:
      - name: Landing Page
        link: /templates/landing-page/
      - name: Content Page
        link: /templates/content-page/
```
