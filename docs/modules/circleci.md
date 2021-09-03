# CircleCI

Displays build information for your CircleCI account.

## Configuration

```yaml
circleci:
  apiKey: "p0d13*********************************************c3"
  enabled: true
  position:
    top: 4
    left: 1
    height: 1
    width: 2
  refreshInterval: 900
```

## Screenshots

<img src="/assets/modules/circleci.png" class="screenshot" width="609" height="150" alt="circleci screenshot" />

## Attributes

<table>
    {% include "attributes/table_header.md" %}

    <tbody>
        {% with name="CircleCI", envvar="WTF_CIRCLE_API_KEY" %}
            {% include "attributes/apikey.md" %}
        {% endwith %}

        
    </tbody>
</table>

{% set src="circleci" %}
{% include "src_path.md" %}