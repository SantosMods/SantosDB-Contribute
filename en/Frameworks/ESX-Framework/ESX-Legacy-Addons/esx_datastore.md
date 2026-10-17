---
title: esx_datastore
description: ESX addon that stores shared and per-player data outside the standard inventory, such as society and property data.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, esx, free, github
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# esx_datastore [![](https://badges.5metrics.dev/esx_datastore/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/esx_datastore)

ESX addon that stores shared and per-player data outside the standard inventory, such as society and property data.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field              | Information     |
| ------------------ | --------------- |
| **Name**           | `esx_datastore` |
| **Creator**        | ESX Framework   |
| **Type**           | Script          |
| **Category**       | Data storage    |
| **Game**           | FiveM           |
| **Price**          | Free            |
| **License**        | GPL-3.0-only    |
| **Framework**      | ESX Legacy      |
| **Version**        | `1.0`           |
| **Legacy Version** | `1.16.0`        |
| **Source**         | GitHub          |
| {.dense}           |                 |

---

## Resource Details {.tabset}

### Overview

`esx_datastore` is similar to `esx_addoninventory` but stores overall data rather than inventory-specific data.

The official documentation defines two datastore types:

* **Shared datastores** do not belong to one user. Example: a police armory.
* **Non-shared datastores** are created for every user when the player loads. Example: `esx_property` outfits.

### Requirements

* `es_extended`
* `esx_lib`
* `oxmysql`

---

## Installation

### Installation Checklist

* [ ] Install and configure ESX
* [ ] Install `oxmysql`
* [ ] Download `esx_datastore` from the official ESX repository
* [ ] Place `esx_datastore` in your server resources
* [ ] Define the datastores your resources need in the database
* [ ] Restart the server after adding datastore definitions
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure es_extended
ensure oxmysql
ensure esx_datastore
```

> A datastore must be configured in the database before a resource uses it. The official documentation requires a server restart afterwards.
> {.is-warning}

---

## Database Configuration

| Field    | Type    | Purpose                                      |
| -------- | ------- | -------------------------------------------- |
| `name`   | string  | Name of the datastore                        |
| `label`  | string  | Label of the datastore (not used)            |
| `shared` | boolean | `1` for a shared datastore or `0` for per-player |
| {.dense} |         |                                              |

## Usage

```lua
TriggerEvent('esx_datastore:getSharedDataStore', 'police', function(store)
    local weapons = store.get('weapons') or {}
end)
```

---

## Links

* [Official Documentation](https://docs.esx-framework.org/en/esx_addons/esx_datastore)
* [Official ESX-Legacy-Addons Repository](https://github.com/esx-framework/ESX-Legacy-Addons)
* [esx_datastore Source](https://github.com/esx-framework/ESX-Legacy-Addons/tree/main/%5Besx_addons%5D/esx_datastore)
* [ESX Framework](https://www.esx-framework.org/)

---

## Credits

Created and maintained through the **ESX Framework** project and its contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.