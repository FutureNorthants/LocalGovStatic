---
layout: page
title: An example content page
---

{% include notification.html title="Example notification" message="This page demonstrates the use of markdown and components." %}

Lorem ipsum dolor sit amet, **consectetur adipiscing** elit. Morbi _ut arcu_ blandit, mattis lacus id, maximus orci. Morbi posuere massa vel dolor lacinia, bibendum congue nunc pharetra. Nulla facilisi. Aliquam a semper velit. Praesent dui tellus, interdum ut venenatis in, dignissim ut nibh.

Morbi venenatis tincidunt lorem. In ac turpis posuere, venenatis nunc consectetur, pretium dolor. Aliquam erat volutpat. Nullam augue metus, faucibus at auctor a, tempus at est. Vivamus id turpis porttitor, volutpat ex ut, facilisis orci.

{% include button.html name="This is a button" link="/example-content-page/" %}

## Heading two

{% include warning-text.html message="This is some warning text!" %}

Fusce interdum at quam in pulvinar. Nunc aliquam risus ac gravida suscipit. Donec eget malesuada erat. Maecenas euismod ipsum eu ante pellentesque pharetra. Praesent porta nulla sodales rhoncus blandit. Pellentesque quis finibus tortor.

{% include video.html youtube="NUmT9pboY5s" label="Northampton bike park" %}

Sed quis ante ac tellus auctor finibus. Vestibulum vehicula viverra aliquet. Cras ut lacus elit. Donec sodales sapien elementum, ultrices mauris id, hendrerit sem.

[View templates](/templates/)

### Example lists

- Duis feugiat est eget dictum dapibus.
- Nulla ex nulla, pellentesque id dui eu, lobortis dapibus enim.
- Aenean varius purus odio, vel cursus sem consequat vestibulum.

1. Duis feugiat est eget dictum dapibus.
1. Nulla ex nulla, pellentesque id dui eu, lobortis dapibus enim.
1. Aenean varius purus odio, vel cursus sem consequat vestibulum.

## Example image component.

{% include image.html image="https://picsum.photos/800/400" alt="An example image" caption="An example image caption" %}

Nullam et leo sollicitudin, interdum nunc nec, consectetur ex. Cras nec rhoncus eros. Nullam fringilla imperdiet urna, ac pulvinar diam venenatis ac.

## Example table

| Example heading | Another heading |
| --------------- | --------------- |
| Some content    | More content    |
| Another row     | Another content |

## Horizontal rule

---

## Example block quote

> Aenean lacinia bibendum nulla sed consectetur. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Donec id elit non mi porta gravida at eget metus. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Donec id elit non mi porta gravida at eget metus. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Etiam porta sem malesuada magna mollis euismod.

_Quote Name_

## Accordion

{% capture accordion_content %}
This is my content that I want to include in my accordion.

- List item 1
- List item 2

Some more text _here_ too.

```yaml
- name: Example
  link: /example/
- name: Example 2
  link: /example-2/
```

{% endcapture %}

{% include accordion.html title="An example accordion" content=accordion_content %}
