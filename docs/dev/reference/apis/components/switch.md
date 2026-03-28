---
title: "Switch API"
linkTitle: "Switch"
weight: 200
type: "docs"
description: "Give commands for getting the state of a physical switch that has two or more discrete positions."
icon: true
images: ["/icons/components/switch.svg"]
date: "2025-02-20"
# updated: ""  # When the content was last entirely checked
---

The switch API allows you to give commands to your [switch components](/operate/reference/components/switch/) for reading the state of a physical switch that has multiple discrete positions.
A simple switch has two positions, and a knob could have any number of positions.

In Go, `switch` is a reserved keyword, so you must alias the import:

```go
import sw "go.viam.com/rdk/components/switch"
```

Then use `sw.FromDependencies(deps, name)` or `sw.FromProvider(machine, name)` to access the switch.

The switch component supports the following methods:

{{< readfile "/static/include/components/apis/generated/switch-table.md" >}}

## API

{{< readfile "/static/include/components/apis/generated/switch.md" >}}
