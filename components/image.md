---
layout: page
title: Image
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

## Markdown

You can include an image using standard markdown:

```markdown
![Alt text](/path-to-image.jpg)
```

This will output the following:

![An example image](https://picsum.photos/800/400)

## Image component

Alternatively, you can use the image component to add a caption to the image.

{% raw %}

```liquid
{% include image.html image="https://picsum.photos/800/800" alt="An example image" caption="An example image caption" %}
```

{% endraw %}

This will output the following:

{% include image.html image="https://picsum.photos/800/800" alt="An example image" caption="An example image caption" %}

### Image component ratio

By default the images will display at 16x9 ratio. This can be overridden by passing in the width and height (from 1 to 16) into the include.

{% raw %}

```liquid
{% include image.html image="https://picsum.photos/800/600" width="4" height="3" alt="An example image" caption="An example image caption" %}
```

{% endraw %}

This will output the following (a 4 by 3 ratio image):

{% include image.html image="https://picsum.photos/800/600" width="4" height="3" alt="An example image" caption="An example image caption" %}
