---
title: BigDaddy-AnimalKingdom
description: Spawns networked wildlife in configurable map zones using animal groups, spawn limits, and PolyZone-defined areas.
published: true
date: 2026-09-13T17:52:48.010Z
tags: script, standalone, animals, ambient-spawns
editor: markdown
dateCreated: 2026-09-13T17:52:48.010Z
---

# Animal Kingdom [![](https://badges.5metrics.dev/BigDaddy-AnimalKingdom/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-AnimalKingdom)

Animal Kingdom spawns networked wildlife in configurable zones around the map.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `Animal Kingdom`         |
| **Resource Folder** | `BigDaddy-AnimalKingdom` |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Script                   |
| **Category**        | Animals                  |
| **Version**         | `v1.0.3`                 |
| **Price**           | $10.00 USD               |
| **Dependency**      | PolyZone                 |
| **QBCore / Qbox**   | ⚠️ Compatibility warning |
| **ESX**             | ⚠️ Compatibility warning |
| {.dense}            |                          |

Big Daddy Scripts marks QBCore, Qbox, and ESX with **⚠️** for Animal Kingdom. This means the Stand-Alone script is expected to work, but framework conflicts may occur.

---

## Resource Details {.tabset}

### Overview

Animal Kingdom creates wildlife spawn zones around the map.

Each zone can use different animal groups and has a configurable maximum number of active animals. Animals are networked so nearby players see the same spawned wildlife.

The included groups cover land, sea, and air animals. Server owners can change animal assignments and create their own zones.

### Features

* Networked wildlife
* Configurable spawn zones
* Configurable animal groups
* Per-zone spawn limits
* Friendly and hostile animal relationships
* Land, sea, and air animals
* Automatic dead-animal cleanup
* Add-on animal support

---

## Requirements

Animal Kingdom requires **PolyZone**.

The purchased ZIP includes a copy of PolyZone for convenience, but Big Daddy Scripts states that PolyZone is a separate project and must be installed separately.

> Four bundled add-on animals, Leopard, Male Lion, Bobcat, and Wolf, require a paid CFX subscription tier that supports add-on peds. Without that entitlement, those animals may spawn invisible.
> {.is-warning}

---

## Installation

### Installation Checklist

* [ ] Download Animal Kingdom from Big Daddy Scripts.
* [ ] Install PolyZone separately.
* [ ] Place `BigDaddy-AnimalKingdom` in your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Add PolyZone before Animal Kingdom in `server.cfg`.
* [ ] Start `BigDaddy-AnimalKingdom`.
* [ ] Restart the server.
* [ ] Check the server and client consoles.

```cfg
ensure PolyZone
start BigDaddy-AnimalKingdom
```

> Do not rename `BigDaddy-AnimalKingdom`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration {.tabset}

### settings.ini

| Setting       | Default | Description                                             |
| ------------- | ------- | ------------------------------------------------------- |
| `key1`        | `none`  | Big Daddy Scripts product key                           |
| `CleanUpDead` | `true`  | Automatically cleans up dead animals                    |
| `ForceDelete` | `true`  | Force-deletes dead animals when someone enters the zone |
| `debug`       | `false` | Debug option intended for support use                   |
| {.dense}      |         |                                                         |

### Animal Groups

Animal groups are defined in `settings.ini` and referenced by `ZONES.json`.

> Big Daddy Scripts warns not to add or remove the predefined animal groups. You can change which animals belong to those groups.
> {.is-warning}

Animal relationships use exact model names and supported relationship values.

Documented relationships include:

```text
HEN
WILD_ANIMAL
SHARK
COUGAR
GUARD_DOG
DOMESTIC_ANIMAL
DEER
```

### zones.json

`zones.json` controls where wildlife can spawn.

A zone includes:

* Unique `zoneId`
* Maximum active animals
* Center coordinates
* Radius
* One or more animal groups

Adding a group multiple times increases its relative chance of selection.

> Big Daddy Scripts specifically warns not to place spaces after commas in the `animalGroups` value.
> {.is-warning}

---

## Files

Big Daddy Scripts recommends leaving these files unchanged unless you understand the effects:

* `peds.meta`
* `PolyZones.lua`

Changing them can break animal or zone behavior.

---

## Usage

No player command is required.

When a player enters a configured zone, Animal Kingdom checks the current wildlife population, performs cleanup when needed, and spawns additional animals up to the configured limit.

Big Daddy Scripts also states that its Delete Ped resource can remove animals spawned by Animal Kingdom.

---

## Compatibility

| Platform        | Status                   |
| --------------- | ------------------------ |
| **Stand-Alone** | Supported                |
| **QBCore**      | ⚠️ Compatibility warning |
| **Qbox**        | ⚠️ Compatibility warning |
| **ESX**         | ⚠️ Compatibility warning |
| **PolyZone**    | Required                 |
| {.dense}        |                          |

---

## Official Links

* [Animal Kingdom Product Page](https://bigdaddyscripts.com/Products/View/2820/Animal-Kingdom)
* [Animal Kingdom Documentation](https://wiki.bigdaddyscripts.com/Documentation/Animal-Kingdom/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

PolyZone is a separate dependency created and maintained by its respective authors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
