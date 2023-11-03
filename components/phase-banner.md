---
layout: page
title: Phase banner
related: components_related
breadcrumbs:
  - name: Components
    link: /components/
---

Add a phase banner to your site by setting the `phase:` in the `_config.yml` file.

```yaml
## For alpha services
phase: ALPHA

## For beta services
phase: BETA
```

Set the link for feedback by setting the `phase_link:` in the `_config.yml` file.

```yaml
## For sending an email
phase_link: mailto:example@example.com?subject=Service name website feedback

## For a link to a form
phase_link: https://example.com/feedback-form
```
