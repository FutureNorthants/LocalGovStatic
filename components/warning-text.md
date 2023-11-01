---
layout: page
title: Warning text
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

A notification component is used to warn users about something important.

You can include the warning text as follows, passing in the message:

{% raw %}

```liquid
{% include warning-text.html message="This is some warning text!" %}
```

{% endraw %}

This will output the following:

{% include warning-text.html message="This is some warning text!" %}
