---
layout: page
title: Notification
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

A notification component is used to tell users about something important, but that is not directly related to the page content.

You can include the notification as follows, passing in the title and the message:

{% raw %}

```liquid
{% include notification.html title="Example notification" message="This is a message for an example notification." %}
```

{% endraw %}

This will output the following:

{% include notification.html title="Example notification" message="This is a message for an example notification." %}
