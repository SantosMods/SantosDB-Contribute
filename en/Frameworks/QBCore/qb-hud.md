---
title: qb-hud
description: QBCore player HUD displaying player, vehicle, money, voice, status, compass, and other gameplay information.
published: true
date: 2026-09-14T01:32:25.983Z
tags: hud, qbcore, script, ui
editor: markdown
dateCreated: 2026-09-14T01:32:25.983Z
---

# qb-hud [![](https://badges.5metrics.dev/qb-hud/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-hud)

QBCore player HUD displaying player, vehicle, money, voice, status, compass, and other gameplay information.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-hud`         |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | HUD              |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | Unknown          |
| **Framework** | QBCore           |
| {.dense}      |                  |

> The current repository does not expose a verified license file or license designation. Do not assume a license from other QBCore resources.
> {.is-warning}

---

## Resource Details {.tabset}

### Overview

`qb-hud` provides the player and vehicle HUD for QBCore.

The current resource handles information including:

* Health
* Armor
* Hunger
* Thirst
* Stress
* Oxygen
* Stamina
* Voice and radio state
* Cash and bank values
* Vehicle speed
* Engine health
* Fuel
* Seatbelt state
* Cruise control
* Nitro
* Harness state
* Altitude
* Compass
* Cinematic mode

### HUD Settings

The HUD includes an in-game settings menu.

The default menu key is `I`. Players can also use:

```text
/menu
```

HUD settings are stored locally.

### Integrations

Current resource code includes integrations with:

* `qb-core`
* `pma-voice`
* `LegacyFuel`
* `InteractSound`

Some features depend on the corresponding integration being installed and configured.

---

## Configuration

Review `config.lua` before starting the resource.

The HUD includes configurable behavior for its menu, display elements, map, vehicle information, and other HUD features.

---

## Usage

Open the HUD menu:

```text
/menu
```

Reset the HUD:

```text
/resethud
```

The default key mapping for the HUD menu is `I`.

---

## Known Issues

The official README documents an error involving:

```text
attempt to index a nil value (global 'Lang')
```

The project recommends obtaining a current QBCore installation through the txAdmin recipe when an existing server contains mismatched resource versions.

The README also notes that map border alignment can be affected by non-default GTA safezone settings.

---

## Compatibility

| Item                  | Information  |
| --------------------- | ------------ |
| **Game**              | FiveM        |
| **Framework**         | QBCore       |
| **Voice integration** | `pma-voice`  |
| **Fuel integration**  | `LegacyFuel` |
| **Resource name**     | `qb-hud`     |
| {.dense}              |              |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-hud)

---

## Before You Install

* [ ] Review `config.lua`
* [ ] Check required integrations for the HUD features you use
* [ ] Test the HUD inside and outside vehicles
* [ ] Test voice, fuel, seatbelt, and status integrations
* [ ] Check the in-game HUD settings menu

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
