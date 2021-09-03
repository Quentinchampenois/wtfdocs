---
title: "CircleCI"
date: 2018-06-10T19:26:08-04:00
draft: false
weight: 20
---

Displays build information for your CircleCI account.

## Configuration

{{< code lang="yaml" >}}
circleci:
  apiKey: "p0d13*********************************************c3"
  enabled: true
  position:
    top: 4
    left: 1
    height: 1
    width: 2
  refreshInterval: 900
  numberOfBuilds: 15
{{< /code >}}

## Screenshots

<img src="/imgs/modules/circleci.png" class="screenshot" width="609" height="150" alt="circleci screenshot" />

{{% attributes %}}
  {{< attributes/apikey name="CircleCI" link="https://circleci.com/account/api" envvar="WTF_CIRCLE_API_KEY" >}}
  {{< attributes/border >}}
  {{< attributes/enabled >}}
  {{< attributes/position >}}
  {{< attributes/refreshInterval >}}
  {{< attributes/custom name="numberOfBuilds" desc="_Optional_ The number of decimal places to display. Default: 10." value="Any positive integer" >}}

{{% /attributes %}}

{{% sourcePath module="circleci" %}}