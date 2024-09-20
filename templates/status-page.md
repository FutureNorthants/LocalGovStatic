---
layout: page
title: Status page
breadcrumbs:
  - name: Templates
    link: /templates
related: templates_related
---

Create a static status page by assigning the `layout: status` in the page's front matter. Create a data file `_data/status.yml` for the page content.

{% include button.html link="/status" name="View an example status page" %}

## Overall status

Set an overall status using the `status:` key in the `status.yml` data file.

Possible values:

- "1" = Operational
- "2" = Performance Issues
- "3" = Partial outage
- "4" = Major outage

```yml
status: "2"
```

## Websites

To show the status of your websites or services, create a `websites:` key in the `status.yml` data file.

Use the below format to list out the name, status (same as overall status values), description and url for each website or service.

```yaml
websites:
  - name: example.com
    status: "1"
    description: The description for the example.com website
    url: https://example.com
```

## Incidents

Create a `incidents:` key in the `status.yml` data file.

Use the below format to list out an incident and it's updates. If you set `highlight: "yes"` then it will appear as a highlighted incident. All incidents from the previous 30 days will be listed under the 'Incidents in the past 30 days' and grouped by date.

You can add as many updates items as you require. The updates description can be in basic markdown format. Take care with the indentation for the updates as .yml files are picky with the indentation.

```yml
incidents:
  - name: staging.example.com outage
    highlight: "yes"
    status: "3"
    start_date: 2024-09-20
    description: An outage with something.
    updates:
      - date_time: 2024-09-20 10:00:00
        description: |
          This is the latest update for this incident. It can be written in markdown. For example, here is a list:
          - List item
          - More detail
      - date_time: 2024-09-20 9:30:00
        description: |
          This is a previous update.
```

### Date formats

- `start_date` should be in the format Y-m-d
- `date_time` should be in the format Y-m-d H:m:s
