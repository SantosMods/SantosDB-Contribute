---
title: qb-weathersync
description: Synchronised time and weather for QBCore with admin commands and exports.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, free, github, weather
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# qb-weathersync [![](https://badges.5metrics.dev/qb-weathersync/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-weathersync)

Synchronised time and weather for QBCore with admin commands and exports.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-weathersync` |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Weather / Time   |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| **Version**   | `2.3.0`          |
| **Source**    | GitHub           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-weathersync` syncs the weather and time for all players and allows editing by command.

### Requirements

* `qb-core`

### Features

* Synced weather for all players
* Synced time
* Commands to freeze time or weather, set weather, set time, and toggle blackout
* Exports such as `nextWeatherStage`

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-weathersync` from the official repository
* [ ] Place `qb-weathersync` in your resources folder
* [ ] Review `config.lua` where present
* [ ] Start `qb-weathersync` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure qb-weathersync
```

---

## Commands

| Command                | Purpose                       |
| ---------------------- | ----------------------------- |
| `/freezetime`          | Toggle time progression       |
| `/freezeweather`       | Toggle dynamic weather        |
| `/weather [type]`      | Set the weather               |
| `/blackout`            | Toggle blackout               |
| `/morning`             | Set time to 9am               |
| `/noon`                | Set time to 12pm              |
| `/evening`             | Set time to 6pm               |
| `/night`               | Set time to 11pm              |
| `/time [hour] (minute)` | Set a custom time            |
| {.dense}               |                               |

Available weather types and defaults are set in `config.lua`.

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-weathersync)
* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-weathersync)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.