---
title: qb-policejob
description: QBCore police job resource with evidence, policing, jail, vehicle, armory, and law-enforcement systems.
published: true
date: 2026-09-14T01:27:37.993Z
tags: jobs, police, qbcore, script
editor: markdown
dateCreated: 2026-09-14T01:27:37.993Z
---

# qb-policejob [![](https://badges.5metrics.dev/qb-policejob/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-policejob)

QBCore police job resource with evidence, policing, jail, vehicle, armory, and law-enforcement systems.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                               |
| -------------- | ------------------------------------------------------------------------- |
| **Name**       | `qb-policejob`                                                            |
| **Creator**    | QBCore Framework                                                          |
| **Type**       | Script                                                                    |
| **Category**   | Police Job                                                                |
| **Game**       | FiveM                                                                     |
| **Price**      | Free                                                                      |
| **License**    | GPL-3.0                                                                   |
| **Framework**  | QBCore                                                                    |
| **Repository** | [qbcore-fivem/qb-policejob](https://github.com/qbcore-fivem/qb-policejob) |
| {.dense}       |                                                                           |

---

## Resource Details {.tabset}

### Overview

`qb-policejob` provides the police job and evidence systems for QBCore.

Features documented by the project include duty controls, armories, fingerprints, evidence storage, police vehicles, speed radars, jail, impounding, GSR, blood drops, bullet casings, handcuffs, emergency-service map visibility, and police radar.

### Requirements

The official repository lists these integrations and dependencies:

* `qb-core`
* `qb-management`
* `qb-garages`
* `qb-clothing`
* `qb-phone`
* `qb-smallresources`
* `qb-menu`
* `qb-input`

The repository also identifies `qb-bossmenu` and `qb-log` as deprecated. `qb-management` replaces `qb-bossmenu`, while logging moved to `qb-smallresources`.

### Commands

The resource includes police commands such as:

```text
/cuff
/escort
/jail
/unjail
/impound
/radar
/911
/911r
/911a
/callsign
```

Refer to the official repository for the complete command list and parameters.

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Install the required supporting QBCore resources
* [ ] Download `qb-policejob`
* [ ] Place `qb-policejob` in your `[qb]` resources
* [ ] Review `config.lua`
* [ ] Add it to your resource startup order
* [ ] Restart the server
* [ ] Test police interactions and evidence systems

### Resource Order

```cfg
ensure qb-core
ensure qb-policejob
```

> Supporting resources used by your configuration must also start in the correct order.
> {.is-info}

---

## Configuration

The resource uses `config.lua` for settings such as:

* Police locations
* Vehicle spawn locations
* Evidence locations
* Armory locations
* Police station blips
* Security cameras
* Police objects
* Helicopter model
* Armory whitelist

Review the current official `config.lua` before changing values.

---

## Compatibility

| Item              | Information    |
| ----------------- | -------------- |
| **Game**          | FiveM          |
| **Framework**     | QBCore         |
| **Job type**      | Police         |
| **Resource name** | `qb-policejob` |
| {.dense}          |                |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-policejob)

---

## Before You Install

* [ ] Replace deprecated dependencies where required
* [ ] Confirm all supporting QBCore resources are installed
* [ ] Review configured police locations
* [ ] Test jail, evidence, armory, garage, and phone integrations

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
