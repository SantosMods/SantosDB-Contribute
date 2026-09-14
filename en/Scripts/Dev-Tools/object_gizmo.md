---
title: object_gizmo
description: FiveM utility that exposes a 3D gizmo for interactively changing an entity's position and rotation.
published: true
date: 2026-09-14T23:56:37.522Z
tags: developer-tool, library, standalone, object-editor
editor: markdown
dateCreated: 2026-09-14T23:56:37.522Z
---

# object_gizmo [![](https://badges.5metrics.dev/object_gizmo/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/object_gizmo)

FiveM utility that exposes a 3D gizmo for interactively changing an entity's position and rotation.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field          | Information       |
| -------------- | ----------------- |
| **Name**       | `object_gizmo`    |
| **Creator**    | DemiAutomatic     |
| **Type**       | Library / Utility |
| **Category**   | Object Editor     |
| **Game**       | FiveM             |
| **License**    | GPL-3.0           |
| **Dependency** | `ox_lib`          |
| {.dense}       |                   |

## Resource Details {.tabset}

### Overview

`object_gizmo` provides a client export for interactively manipulating an entity's position and rotation with a 3D gizmo.

The current manifest declares:

```text
ox_lib
```

as a dependency.

### Export

```lua
exports.object_gizmo:useGizmo(handle)
```

The result contains the entity handle, final position, and final rotation.

### Controls

| Key      | Action                  |
| -------- | ----------------------- |
| `W`      | Translate mode          |
| `R`      | Rotate mode             |
| `S`      | Scale mode when enabled |
| `Q`      | Relative / world mode   |
| `LAlt`   | Snap to ground          |
| `Enter`  | Finish editing          |
| {.dense} |                         |

### Test Command

The resource includes:

```text
testGizmo
```

for demonstrating the gizmo.

## Installation

### Installation Checklist

* [ ] Install `ox_lib`
* [ ] Download `object_gizmo`
* [ ] Place it in your resources directory
* [ ] Start `ox_lib`
* [ ] Start `object_gizmo`
* [ ] Test `testGizmo`
* [ ] Integrate `useGizmo` into the consuming resource

```cfg
ensure ox_lib
ensure object_gizmo
```

> The gizmo only works on entities the user has sufficient permission to manipulate.
> {.is-info}

## Links

* [Official GitHub Repository](https://github.com/DemiAutomatic/object_gizmo)
* [Official Releases](https://github.com/DemiAutomatic/object_gizmo/releases)

## Credits

Created and maintained by **DemiAutomatic** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
