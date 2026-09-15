---
title: PolyZone
description: FiveM zone library for defining shapes and testing whether points are inside or outside configured zones.
published: true
date: 2026-09-14T01:40:58.899Z
tags: developer-tool, script, standalone, zones
editor: markdown
dateCreated: 2026-09-14T01:40:58.899Z
---

# PolyZone [![](https://badges.5metrics.dev/PolyZone/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/PolyZone)

FiveM zone library for defining shapes and testing whether points are inside or outside configured zones.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `PolyZone`       |
| **Creator**   | mkafrin          |
| **Type**      | Script / Library |
| **Category**  | Zones            |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | MIT              |
| **Framework** | Standalone       |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`PolyZone` defines zones with different shapes and tests whether a point is inside or outside a zone.

The repository contains implementations including:

* `BoxZone.lua`
* `CircleZone.lua`
* `ComboZone.lua`
* `EntityZone.lua`
* `PolyZone`

### Requirements

Scripts using `PolyZone` must include the required zone files in their resource manifest.

Some zone implementations depend on other files.

For example, the official documentation notes that `EntityZone.lua` requires `BoxZone.lua`, which in turn requires `client.lua`.

### Debugging

Poly zones support debugging options such as:

```lua
debugPoly = true
debugGrid = true
```

Other zone types support `debugPoly`.

---

## Installation

### Installation Checklist

* [ ] Download the official release
* [ ] Place `PolyZone` in your resources folder
* [ ] Start `PolyZone`
* [ ] Include the required PolyZone scripts in resources that use the library
* [ ] Verify zone dependencies
* [ ] Test zones with debugging enabled when needed

### Resource Order

```cfg
ensure PolyZone
```

---

## Usage

At minimum, resources using the base PolyZone functionality must include `client.lua`.

Include additional zone files required by the zone type your resource uses.

> Missing required zone scripts can cause `attempt to index a nil value` errors when creating zones.
> {.is-warning}

---

## Compatibility

| Item              | Information |
| ----------------- | ----------- |
| **Game**          | FiveM       |
| **Framework**     | Standalone  |
| **Language**      | Lua         |
| **Resource name** | `PolyZone`  |
| {.dense}          |             |

---

## Links

* [Official GitHub Repository](https://github.com/mkafrin/PolyZone)
* [Official Releases](https://github.com/mkafrin/PolyZone/releases)
* [Official Wiki](https://github.com/mkafrin/PolyZone/wiki)

---

## Before You Install

* [ ] Identify the zone types your resources require
* [ ] Include every required Lua file
* [ ] Check `minZ` and `maxZ` when using vertical bounds
* [ ] Check point order when manually creating polygons
* [ ] Use debug drawing when troubleshooting zones

---

## Credits

Created by **mkafrin** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
