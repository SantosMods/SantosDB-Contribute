---
title: qb-inventory
description: Slot-based QBCore inventory system with stashes, vehicle storage, weapon attachments, shops, and item drops.
published: true
date: 2026-09-14T01:28:19.636Z
tags: inventory, qbcore, script, stashes
editor: markdown
dateCreated: 2026-09-14T01:28:10.725Z
---

# qb-inventory [![](https://badges.5metrics.dev/qb-inventory/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-inventory)

Slot-based QBCore inventory system with stashes, vehicle storage, weapon attachments, shops, and item drops.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                               |
| -------------- | ------------------------------------------------------------------------- |
| **Name**       | `qb-inventory`                                                            |
| **Creator**    | QBCore Framework                                                          |
| **Type**       | Script                                                                    |
| **Category**   | Inventory                                                                 |
| **Game**       | FiveM                                                                     |
| **Price**      | Free                                                                      |
| **License**    | GPL-3.0                                                                   |
| **Framework**  | QBCore                                                                    |
| **Repository** | [qbcore-fivem/qb-inventory](https://github.com/qbcore-fivem/qb-inventory) |
| {.dense}       |                                                                           |

---

## Resource Details {.tabset}

### Overview

`qb-inventory` is the slot-based inventory system used with QBCore.

The official repository documents support for:

* Personal and shared stashes
* Vehicle trunks
* Vehicle gloveboxes
* Weapon attachments
* Shops
* Item drops

### Requirements

* `qb-core`
* `qb-smallresources` for transfer and history logging

### Database

The repository includes:

* `qb-inventory.sql`
* `migrate.sql`

A database import is required for installation.

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Install `qb-smallresources`
* [ ] Download `qb-inventory`
* [ ] Place it in the `[qb]` directory
* [ ] Import `qb-inventory.sql`
* [ ] Add the resources to your startup configuration
* [ ] Restart the server
* [ ] Test player, stash, vehicle, and shop inventories

### Resource Order

```cfg
ensure qb-core
ensure qb-smallresources
ensure qb-inventory
```

---

## Migration

> Back up your database before migrating an existing inventory installation.
> {.is-danger}

The repository provides `migrate.sql` for migrating saved inventory data from older storage tables.

Follow the current repository migration instructions before removing old inventory tables.

---

## Configuration

Configuration files are stored under the repository's `config` directory.

Review the official configuration before changing inventory behavior, shops, or related features.

---

## Compatibility

| Item               | Information    |
| ------------------ | -------------- |
| **Game**           | FiveM          |
| **Framework**      | QBCore         |
| **Database setup** | Required       |
| **Resource name**  | `qb-inventory` |
| {.dense}           |                |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-inventory)

---

## Before You Install

* [ ] Back up your database
* [ ] Install `qb-smallresources`
* [ ] Import the current SQL schema
* [ ] Follow migration instructions if replacing an older version
* [ ] Test stashes, trunks, gloveboxes, shops, and item drops

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
