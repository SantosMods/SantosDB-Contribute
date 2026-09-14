---
title: bob74_ipl
description: FiveM resource that loads missing map IPLs and provides functions for customizing GTA V interiors.
published: true
date: 2026-09-14T01:40:17.363Z
tags: script, standalone, interiors, ipl
editor: markdown
dateCreated: 2026-09-14T01:40:17.363Z
---

# bob74_ipl [![](https://badges.5metrics.dev/bob74_ipl/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/bob74_ipl)

FiveM resource that loads missing map IPLs and provides functions for customizing GTA V interiors.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information     |
| ------------- | --------------- |
| **Name**      | `bob74_ipl`     |
| **Creator**   | Bob74           |
| **Type**      | Script          |
| **Category**  | Map / Interiors |
| **Game**      | FiveM           |
| **Price**     | Free            |
| **License**   | MIT             |
| **Framework** | Standalone      |
| {.dense}      |                 |

---

## Resource Details {.tabset}

### Overview

`bob74_ipl` loads map areas and IPLs that GTA V does not load by default.

The resource can also customize story mode and GTA Online interiors from other resources.

The official Wiki documents the available functions and default values for supported interiors.

### Framework Support

`bob74_ipl` does not require a roleplay framework.

### Releases

The project instructs users to download the latest official release rather than relying on an arbitrary repository snapshot.

---

## Installation

### Installation Checklist

* [ ] Download the latest official release
* [ ] Extract `bob74_ipl.zip`
* [ ] Place `bob74_ipl` in your resources folder
* [ ] Add it to `server.cfg`
* [ ] Restart the server
* [ ] Check configured interiors in-game

### Resource Order

```cfg
start bob74_ipl
```

---

## Configuration

The project Wiki documents customization functions for supported interiors.

Default configurations can be loaded through the relevant interior API, including functions following this pattern:

```lua
IPL_NAME.LoadDefault()
```

Use the documentation for the exact function names available for each interior.

---

## Compatibility

| Item              | Information                 |
| ----------------- | --------------------------- |
| **Game**          | FiveM                       |
| **Framework**     | Standalone                  |
| **Purpose**       | IPL and interior management |
| **Resource name** | `bob74_ipl`                 |
| {.dense}          |                             |

---

## Links

* [Official GitHub Repository](https://github.com/Bob74/bob74_ipl)
* [Official Releases](https://github.com/Bob74/bob74_ipl/releases/latest)
* [Official Wiki](https://github.com/Bob74/bob74_ipl/wiki)

---

## Before You Install

* [ ] Use the latest official release
* [ ] Review the Wiki before customizing interiors
* [ ] Check other map resources for overlapping IPL changes
* [ ] Test modified interiors after configuration changes

---

## Credits

Created by **Bob74** and project contributors.

The project states that its original work was based on Mikeeh's IPL loading script.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
