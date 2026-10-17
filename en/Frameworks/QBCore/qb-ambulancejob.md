---
title: qb-ambulancejob
description: EMS job, death, and wounding system for the QBCore framework.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, free, github, ems
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# qb-ambulancejob [![](https://badges.5metrics.dev/qb-ambulancejob/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-ambulancejob)

EMS job, death, and wounding system for the QBCore framework.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information       |
| ------------- | ----------------- |
| **Name**      | `qb-ambulancejob` |
| **Creator**   | QBCore Framework  |
| **Type**      | Script            |
| **Category**  | EMS Job           |
| **Game**      | FiveM             |
| **Price**     | Free              |
| **License**   | GPL-3.0           |
| **Framework** | QBCore            |
| **Version**   | `1.2.4`           |
| **Source**    | GitHub            |
| {.dense}      |                   |

---

## Resource Details {.tabset}

### Overview

`qb-ambulancejob` provides the EMS job and the death and wound logic for QBCore. The manifest describes it as a player health, death, and wounding system with an EMS job.

### Requirements

* `qb-core`
* `qb-phone`
* `PolyZone`
* `oxmysql`
* `qb-target` (optional)

### Features

* EMS job
* Death and last-stand logic
* Wounding system
* Target or draw-text interaction through the `UseTarget` convar

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Install `qb-phone`
* [ ] Install `PolyZone`
* [ ] Install `oxmysql`
* [ ] Download `qb-ambulancejob` from the official repository
* [ ] Place `qb-ambulancejob` in your resources folder
* [ ] Review `config.lua` where present
* [ ] Start `qb-ambulancejob` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure PolyZone
ensure qb-phone
ensure qb-ambulancejob
```

---

## Configuration

Choose the interaction style with a convar:

```cfg
setr UseTarget false
```

Use `true` to enable `qb-target` interactions.

## Medal Clip Capture

The official README states that the resource asks Medal to save a clip when a player goes down, and that this is enabled by default. It only affects players who run Medal, and the resource uploads nothing itself.

Disable it in `config.lua`:

```lua
Config.Medal = { Enabled = false }
```

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-ambulancejob)
* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-ambulancejob)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.