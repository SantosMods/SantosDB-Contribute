---
title: qb-garages
description: QBCore garage system for public, house, job, gang, and depot vehicle storage.
published: true
date: 2026-09-14T01:33:21.874Z
tags: garage, qbcore, script, vehicles
editor: markdown
dateCreated: 2026-09-14T01:33:21.874Z
---

# qb-garages [![](https://badges.5metrics.dev/qb-garages/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-garages)

QBCore garage system for public, house, job, gang, and depot vehicle storage.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-garages`     |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Garages          |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-garages` manages vehicle storage for QBCore.

The resource supports:

* Public garages
* House garages
* Gang garages
* Job garages
* Depot garages
* Ground vehicles
* Water vehicles
* Air vehicles

### Public Garages

Public garages store owned vehicles.

Players can only park vehicles they own in public garages.

### House Garages

House garages integrate with the QBCore housing system.

Players with access to a house garage can store and retrieve eligible vehicles.

### Job and Gang Garages

The resource supports job-specific and gang-specific garages.

`SharedGarages` controls whether job and gang garages operate as shared or personal garages.

### Depot

Depot garages handle impounded vehicles.

Police can use:

```text
/depot [price]
```

to send a vehicle to the depot.

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-garages`
* [ ] Place `qb-garages` in your `[qb]` resources
* [ ] Review `player_vehicles.sql`
* [ ] Review `config.lua`
* [ ] Add the resource to your startup configuration
* [ ] Restart the server
* [ ] Test each configured garage type

### Resource Order

```cfg
ensure qb-core
ensure qb-garages
```

---

## Configuration

The official documentation exposes settings including:

```lua
AutoRespawn = false
SharedGarages = false
VisuallyDamageCars = true
```

Garage entries can define properties including:

* Label
* Vehicle withdrawal point
* Spawn point
* Storage point
* Blip visibility
* Blip name
* Blip number
* Garage type
* Vehicle type

Supported vehicle types documented by the project are:

```text
car
sea
air
```

Garage types include public, job, gang, and depot configurations.

---

## Compatibility

| Item                | Information  |
| ------------------- | ------------ |
| **Game**            | FiveM        |
| **Framework**       | QBCore       |
| **Ground vehicles** | Supported    |
| **Water vehicles**  | Supported    |
| **Air vehicles**    | Supported    |
| **Resource name**   | `qb-garages` |
| {.dense}            |              |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-garages)
* [Official QBCore Documentation](https://docs.qbcore.org/qbcore-documentation/qbcore-resources/qb-garages)

---

## Before You Install

* [ ] Review existing vehicle database data
* [ ] Configure garage locations
* [ ] Choose your `AutoRespawn` behavior
* [ ] Choose your `SharedGarages` behavior
* [ ] Test public, job, gang, house, and depot garages that your server uses

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
