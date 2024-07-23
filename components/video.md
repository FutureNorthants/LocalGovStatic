---
layout: page
title: Video
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

A video component can be used to embed a video, with the benefit of it keeping a responsive 16 by 9 ratio.

## YouTube

You can include a YouTube video as follows, passing in the video id and the descriptive label:

{% raw %}

```liquid
{% include video.html youtube="NUmT9pboY5s" label="Northampton bike park" %}
```

{% endraw %}

This will output the following:

{% include video.html youtube="NUmT9pboY5s" label="Northampton bike park" %}

## TikTok

You can include a TikTok video as follows, passing in the video id and the descriptive label:

{% raw %}

```liquid
{% include video.html tiktok="7390064283612106016" label="Northampton market square" %}
```

{% endraw %}

This will output the following:

{% include video.html tiktok="7390064283612106016" label="Northampton market square" %}
