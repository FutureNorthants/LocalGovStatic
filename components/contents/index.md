---
layout: page
title: Contents
related: components_related
contents: example_contents
breadcrumbs:
  - name: Components
    link: /components/
---

This page displays the example contents. The contents links will be inserted at the top of the page and the next and previous navigation will be added to the bottom of the page.

All pages in the contents will have the `<h1>` tag as the contents title and then the `<h2>` tag from the current page's title will be displayed underneath

Create a contents file in the `_data` directory with the following format:

```yaml
title: Contents example
links:
  - name: Overview
    link: /components/contents/
  - name: An example sub page
    link: /components/contents/an-example-sub-page/
  - name: Another example sub page
    link: /components/contents/another-example-sub-page/
```

Then update the page's front matter, setting the `contents:` to the filename without the extension.

For example, if the file was named `example_contents.yml` then set the page's front matter to `contents: example_contents`.
