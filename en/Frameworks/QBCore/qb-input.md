---
title: qb-input
description: NUI input form system for the QBCore framework, based on NH Keyboard by NeroHiro.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, free, github, ui
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# qb-input [![](https://badges.5metrics.dev/qb-input/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-input)

NUI input form system for the QBCore framework, based on NH Keyboard by NeroHiro.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-input`       |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Input / Dialog   |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| **Version**   | `1.2.0`          |
| **Source**    | GitHub           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-input` shows an input form and returns the entered values. The README states that it is a modified version of NH Keyboard by NeroHiro.

### Requirements

* `qb-core`

### Features

* Input types: text, password, number, radio, checkbox, select, and color
* Required and optional fields
* Default values

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-input` from the official repository
* [ ] Place `qb-input` in your resources folder
* [ ] Review `config.lua` where present
* [ ] Start `qb-input` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure qb-input
```

---

## Usage

```lua
local dialog = exports['qb-input']:ShowInput({
    header = "Test",
    submitText = "Bill",
    inputs = {
        { text = "Citizen ID (#)", name = "citizenid", type = "text", isRequired = true },
    }
})
```

Input types must be lowercase.

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-input)
* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-input)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.