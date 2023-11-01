---
layout: page
title: Related links
related: navigation_related
breadcrumbs:
  - name: Components
    link: /components/
---

To add links to other related pages, add the `related:` to the front matter, with the value set as the filename of the related links in the `_data` directory.

The related links data file should be in the following format:

```yaml
- name: My link
  link: /my-page-link/
- name: My other link
  link: /my-other-link/
```

The related links will appear on the right sidebar of a page. This will only show when `layout: page` is set in the page's front matter.

It will detect if the current page is in the list of related links. The current page will show as plain text instead of a link.
