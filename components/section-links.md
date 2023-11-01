---
layout: page
title: Section links
related: navigation_related
breadcrumbs:
  - name: Components
    link: /components/
---

Section links are added by setting the `sections:` in the pages front matter that corresponds to a matching file in the `_data` directory.

The data file should be in the following format:

```yaml
- title: First section
  links:
    - name: Example Page
      link: /first-section/example-page/
      summary: An example landing page
    - name: Second Example page
      link: /first-section/second-example-page
      summary: An example content page
```

You can have multiple sections in the data file.

```yaml
- title: First section
  links:
    - name: Example Page
      link: /first-section/example-page/
      summary: An example landing page
    - name: Second Example page
      link: /first-section/second-example-page
      summary: An example content page
- title: Second section
  links:
    - name: Example Page
      link: /second-section/example-page/
      summary: An example landing page
    - name: Second Example page
      link: /second-section/second-example-page
      summary: An example content page
```

[View example landing page](/templates/landing-page/)

## Section links with images

```yaml
- title: First section
  links:
    - name: Example Page
      link: /first-section/example-page/
      summary: An example landing page
      image: https://picsum.photos/400/300
    - name: Second Example page
      link: /first-section/second-example-page
      summary: An example content page
      image: https://picsum.photos/400/300
```
