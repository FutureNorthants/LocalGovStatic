---
layout: page
title: File download
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

To improve the appearance of a file download, use the following:

{% raw %}

```liquid
{% include file-download.html url="/path-to-download.pdf" title="Example file" size="1.0MB" type="PDF" %}
```

{% endraw %}

This will output the following:

{% include file-download.html url="/" title="Example file" size="1.0MB" type="PDF" %}
