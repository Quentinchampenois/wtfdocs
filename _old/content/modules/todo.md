---
title: "Todo"
date: 2018-05-10T12:41:50-07:00
draft:  false
weight: 220
---

An interactive todo list.

## Configuration

{{< code lang="yaml" >}}
todo:
  checkedIcon: "X"
  colors:
    checked: gray
    highlight:
      fore: "black"
      back: "orange"
  enabled: true
  filename: "todo.yml"
  position:
    top: 2
    left: 2
    height: 2
    width: 1
  refreshInterval: 3600
{{< /code >}}

## Screenshots

<img class="screenshot" src="/imgs/modules/todo.png" width="320" height="388" alt="todo screenshot" />

{{% attributes %}}
  {{< attributes/border >}}
  {{< attributes/colors/custom name="checked" desc="The foreground color for checked rows.">}}
  {{< attributes/colors/highlight >}}
  {{< attributes/custom name="checkedIcon" desc="<i>Optional</i> The icon used to denote a 'checked' todo item." value="Any displayable unicode character." >}}
  {{< attributes/enabled >}}
  {{< attributes/custom name="filename" desc="The name for the todo file." value="Any valid filename, ideally ending in `yml`." >}}
  {{< attributes/focusChar >}}
  {{< attributes/position >}}
  {{< attributes/refreshInterval >}}
{{% /attributes %}}

{{% keyboard %}}
  {{< keyboard/foreSlash >}}
  {{< keyboard/esc desc="Remove focus from the selected item" >}}
  {{< keyboard/esc desc="Close the modal item dialog without saving changes" >}}
  {{< keyboard/return desc="Edit the selected item" >}}
  {{< keyboard/return desc="Close the modal item dialog and save changes" >}}
  {{< keyboard/space desc="Check/uncheck the selected item" >}}

  {{< keyboard/spacer >}}

  {{< keyboard/j >}}
  {{< keyboard/k >}}
  {{< keyboard/n desc="Create a new list item" >}}
  {{< keyboard/o desc="Opens the todo list file in whichever text editor is associated with that file type" >}}
  {{< keyboard/r >}}

  {{< keyboard/spacer >}}

  {{< keyboard/arrowDown >}}
  {{< keyboard/arrowUp >}}

  {{< keyboard/spacer >}}

  {{< keyboard/ctrlD >}}
  {{< keyboard/custom name="Ctrl-j" desc="Move the selected item down the list" >}}
  {{< keyboard/custom name="Ctrl-k" desc="Move the selected item up the list" >}}
{{% /keyboard %}}

{{% sourcePath module="todo" %}}