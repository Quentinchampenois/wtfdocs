---
title: "Docker"
date: 2019-09-07T06:51:00-07:00
draft: false
weight: 63
---

<img src="/imgs/services/docker.png" width="128" height="97" alt="docker" title="docker" style="float: left; padding-right: 8px;" />

Displays information about currently-running Docker processes.

## Configuration

{{< code lang="yaml" >}}
docker:
  type: docker
  enabled: true
  labelColor: lightblue
  position:
    top: 0
    left: 0
    height: 3
    width: 3
  refreshInterval: 1
{{< /code >}}

## Screenshots

<img class="screenshot" src="/imgs/modules/docker.png" width="275" height="320" alt="github screenshot" />

{{% attributes %}}
  {{< attributes/enabled >}}
  {{< attributes/colors/custom name="labelColor" desc="The color to display the row labels in." >}}
  {{< attributes/position >}}
  {{< attributes/refreshInterval >}}
  {{< attributes/title >}}
{{% /attributes %}}

{{% sourcePath module="docker" %}}