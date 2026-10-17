---
title: qb-vehiclekeys
description: Vehicle keys system for QBCore that manages vehicle doors and lets players lock and unlock vehicles.
published: true
date: 2026-10-16T18:00:00.000Z
tags: script, qbcore, free, github, vehicles
editor: markdown
dateCreated: 2026-10-16T18:00:00.000Z
---

# qb-vehiclekeys [![](https://badges.5metrics.dev/qb-vehiclekeys/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-vehiclekeys)

Vehicle keys system for QBCore that manages vehicle doors and lets players lock and unlock vehicles.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-vehiclekeys` |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Vehicle Keys     |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| **Version**   | `1.6.0`          |
| **Source**    | GitHub           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-vehiclekeys` manages vehicle doors and keys so that players can lock and unlock vehicles. The README notes that other resources should use the documented server exports instead of triggering internal events.

### Requirements

* `qb-core`

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-vehiclekeys` from the official repository
* [ ] Place `qb-vehiclekeys` in your resources folder
* [ ] Review `config.lua`
* [ ] Start `qb-vehiclekeys` after `qb-core`
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure qb-vehiclekeys
```

---

## Server Exports

```lua
exports['qb-vehiclekeys']:GiveKeys(source, plate)
exports['qb-vehiclekeys']:RemoveKeys(source, plate)
exports['qb-vehiclekeys']:HasKeys(source, plate)
```

`GiveKeys` uses the vehicle the player is in when no plate is given.

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-vehiclekeys)
* [GitHub Repository](https://github.com/qbcore-fivem/qb-vehiclekeys)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.