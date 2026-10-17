---
title: qb-menu
description: Menu system for the QBCore framework, based on NH Context by NeroHiro.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, free, github, menus, ui
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# qb-menu [![](https://badges.5metrics.dev/qb-menu/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-menu)

Menu system for the QBCore framework, based on NH Context by NeroHiro.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-menu`        |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Menus            |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| **Version**   | `1.5.0`          |
| **Source**    | GitHub           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-menu` is a context menu that other QBCore resources use to present options. The README states that it is a modified version of NH Context by NeroHiro.

### Requirements

* `qb-core`

### Features

* Menu items with a header and description
* Non-clickable menu headers
* Disabled items
* Events, server events, commands, QBCore commands, or functions as actions

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-menu` from the official repository
* [ ] Place `qb-menu` in your resources folder
* [ ] Review `config.lua` where present
* [ ] Start `qb-menu` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure qb-menu
```

---

## Usage

```lua
exports["qb-menu"]:openMenu({
    { header = "Main Title", isMenuHeader = true },
    { header = "Sub Menu Button", txt = "This goes to a sub menu", params = { event = "qb-menu:client:testMenu2", args = { number = 1 } } },
})
```

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-menu)
* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-menu)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.