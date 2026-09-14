---
title: qb-target
description: FiveM targeting system for interacting with predefined entities, models, entity types, and PolyZones.
published: true
date: 2026-09-14T01:27:00.281Z
tags: qbcore, script, target, interaction
editor: markdown
dateCreated: 2026-09-14T01:27:00.281Z
---

# qb-target [![](https://badges.5metrics.dev/qb-target/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-target)

FiveM targeting system for interacting with predefined entities, models, entity types, and PolyZones.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                         |
| -------------- | ------------------------------------------------------------------- |
| **Name**       | `qb-target`                                                         |
| **Creator**    | QBCore Framework                                                    |
| **Type**       | Script                                                              |
| **Category**   | Target / Interaction                                                |
| **Game**       | FiveM                                                               |
| **Price**      | Free                                                                |
| **License**    | GPL-3.0                                                             |
| **Framework**  | QBCore optional                                                     |
| **Repository** | [qbcore-fivem/qb-target](https://github.com/qbcore-fivem/qb-target) |
| {.dense}       |                                                                     |

---

## Resource Details {.tabset}

### Overview

`qb-target` provides target-based interactions with predefined entities, models, entity types, and PolyZones.

Target options can trigger events, functions, or commands and can use distance, job, gang, citizen ID, item, entity, or `canInteract` checks.

### Requirements

Required dependency:

* `PolyZone`

Optional dependency:

* `qb-core`

### Features

* Entity, model, entity type, and zone targeting
* Per-option interaction distance
* Events, functions, and command actions
* Job and gang checks
* Citizen ID and item checks
* Entity bone support
* `canInteract` conditions
* Ped spawning with target options

---

## Installation

### Installation Checklist

* [ ] Install `PolyZone`
* [ ] Download `qb-target`
* [ ] Place `qb-target` in your resources folder
* [ ] Review `config.lua`
* [ ] Start dependencies first
* [ ] Start `qb-target`
* [ ] Restart the server
* [ ] Check the console for errors

### Resource Order

```cfg
ensure PolyZone
ensure qb-target
```

If your configuration uses QBCore integration:

```cfg
ensure qb-core
ensure PolyZone
ensure qb-target
```

---

## Configuration

The repository includes:

* `config.lua`
* `EXAMPLES.md`
* `TEMPLATES.md`

Use the official examples and templates when adding target interactions.

---

## Compatibility

| Item                    | Information          |
| ----------------------- | -------------------- |
| **Game**                | FiveM                |
| **QBCore**              | Optional integration |
| **Required dependency** | `PolyZone`           |
| **Resource name**       | `qb-target`          |
| {.dense}                |                      |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-target)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The project credits `qtarget`, `bt-target`, and `ms-peds` for work used in or related to the resource.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
