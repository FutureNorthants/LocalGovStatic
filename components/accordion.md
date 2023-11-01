---
layout: page
title: Accordion
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

## Basic accordion

To insert a basic accordion, set the title and the content in the include tag.

{% raw %}

```liquid
{% include accordion.html title="Accordion title" content="This is the accordion content" %}
```

{% endraw %}

This will output the following:

{% include accordion.html title="Accordion title" content="This is the accordion content" %}

## Advanced content

To insert longer, or more complicated content into the accordion, use the liquid `capture` tag to capture the content and then pass it into the include tag as a variable.

Using `capture` allows you to use markdown and format the content.

{% raw %}

```liquid
{% capture accordion_content %}
This is my content that I want to include in my accordion.

- List item 1
- List item 2

Some more text _here_ too.

{% endcapture %}

{% include accordion.html title="Advanced accordion" content=accordion_content %}
```

{% endraw %}

This will output the following:

{% capture accordion_content %}
This is my content that I want to include in my accordion.

- List item 1
- List item 2

Some more text _here_ too.

{% endcapture %}

{% include accordion.html title="Advanced accordion" content=accordion_content %}
