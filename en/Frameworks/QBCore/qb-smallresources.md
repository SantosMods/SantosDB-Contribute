---
title: qb-smallresources
description: Collection of small QBCore gameplay resources and utility features combined into one resource.
published: true
date: 2026-09-14T01:29:44.101Z
tags: qbcore, script, utility, gameplay
editor: markdown
dateCreated: 2026-09-14T01:29:44.101Z
---

# qb-smallresources [![](https://badges.5metrics.dev/qb-smallresources/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-smallresources)

Collection of small QBCore gameplay resources and utility features combined into one resource.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                                         |
| -------------- | ----------------------------------------------------------------------------------- |
| **Name**       | `qb-smallresources`                                                                 |
| **Creator**    | QBCore Framework                                                                    |
| **Type**       | Script                                                                              |
| **Category**   | Utilities                                                                           |
| **Game**       | FiveM                                                                               |
| **Price**      | Free                                                                                |
| **License**    | GPL-3.0                                                                             |
| **Framework**  | QBCore                                                                              |
| **Dependency** | `qb-core`                                                                           |
| **Repository** | [qbcore-fivem/qb-smallresources](https://github.com/qbcore-fivem/qb-smallresources) |
| {.dense}       |                                                                                     |

---

## Resource Details {.tabset}

### Overview

`qb-smallresources` combines multiple small QBCore gameplay and utility systems into one resource.

### Requirements

* `qb-core`

### Features

The official repository documents features including:

* Consumable food, drinks, alcohol, and drugs
* Drug effects
* Default weapon-drop removal
* Default vehicle-spawn removal
* Emergency NPC removal
* Wanted-system removal
* Binoculars
* Weapon draw animations
* Teleport markers
* Hostage interactions
* Pointing
* Seatbelt and cruise control
* Parachutes
* Armor
* Weapon recoil
* Tackling
* NPC aggression adjustments
* Race harness
* `/id`
* Population density adjustments
* HUD removal
* Fireworks
* Discord rich presence
* Crouch and prone

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-smallresources`
* [ ] Place it in the `[qb]` directory
* [ ] Review its configuration
* [ ] Add it after `qb-core`
* [ ] Restart the server
* [ ] Test the features you intend to use

### Resource Order

```cfg
ensure qb-core
ensure qb-smallresources
```

---

## Configuration

The project separates many features into files related to their function.

Review each feature's configuration before enabling or changing gameplay behavior.

> `qb-smallresources` changes multiple gameplay systems. Test changes on a development server before deploying them to production.
> {.is-warning}

---

## Usage

One documented command is:

```text
/id
```

This displays the player's ID.

Other functionality runs through configured gameplay systems rather than a single command interface.

---

## Compatibility

| Item              | Information         |
| ----------------- | ------------------- |
| **Game**          | FiveM               |
| **Framework**     | QBCore              |
| **Dependency**    | `qb-core`           |
| **Resource name** | `qb-smallresources` |
| {.dense}          |                     |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-smallresources)

---

## Before You Install

* [ ] Review every feature you plan to use
* [ ] Check for overlap with other gameplay resources
* [ ] Confirm population and HUD changes match your server setup
* [ ] Test vehicle, weapon, consumable, and animation behavior

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
