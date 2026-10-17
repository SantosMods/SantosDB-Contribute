---
title: esx_society
description: ESX addon for job society management, including employee management, society bank accounts, and money washing.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, esx, free, github, jobs, banking
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# esx_society [![](https://badges.5metrics.dev/esx_society/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/esx_society)

ESX addon for job society management, including employee management, society bank accounts, and money washing.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field              | Information    |
| ------------------ | -------------- |
| **Name**           | `esx_society`  |
| **Creator**        | ESX Framework  |
| **Type**           | Script         |
| **Category**       | Society / Jobs |
| **Game**           | FiveM          |
| **Price**          | Free           |
| **License**        | GPL-3.0-only   |
| **Framework**      | ESX Legacy     |
| **Version**        | `1.0`          |
| **Legacy Version** | `1.16.0`       |
| **Source**         | GitHub         |
| {.dense}           |                |

---

## Resource Details {.tabset}

### Overview

`esx_society` adds society management to ESX: hire, fire, promote or demote employees, change salaries, and manage society bank accounts and money washing.

### Requirements

* `es_extended`
* `esx_lib`
* `cron`
* `esx_addonaccount`
* `oxmysql`

### Features

* Employee management (hire, fire, promote, demote)
* Salary changes
* Society bank accounts
* Money washing
* Boss menu with per-feature options

---

## Installation

### Installation Checklist

* [ ] Install and configure ESX
* [ ] Install `cron`, `esx_addonaccount`, and `oxmysql`
* [ ] Download `esx_society` from the official ESX repository
* [ ] Place `esx_society` in your server resources
* [ ] Review `config.lua`
* [ ] Start `esx_society` before every resource that uses societies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure es_extended
ensure oxmysql
ensure esx_addonaccount
ensure esx_society
```

> Start `esx_society` before all resources that use societies. The official documentation warns that many things go wrong otherwise.
> {.is-warning}

---

## Configuration

| Option                     | Default              | Purpose                                      |
| -------------------------- | -------------------- | -------------------------------------------- |
| `Config.EnableESXIdentity` | `true`               | Enable when using ESX Identity               |
| `Config.MaxSalary`         | `3500`               | Maximum salary that can be set               |
| `Config.BossGrades`        | `{ ['boss'] = true }` | Grade names treated as bosses               |
| {.dense}                   |                      |                                              |

## Registering a Society

```lua
exports["esx_society"]:registerSociety('mechanic', 'Mechanic', 'society_mechanic', 'society_mechanic', 'society_mechanic', {type = 'private'})
```

The `type` option can be `public` or `private`.

---

## Links

* [Official Documentation](https://docs.esx-framework.org/en/esx_addons/esx_society)
* [Official ESX-Legacy-Addons Repository](https://github.com/esx-framework/ESX-Legacy-Addons)
* [esx_society Source](https://github.com/esx-framework/ESX-Legacy-Addons/tree/main/%5Besx_addons%5D/esx_society)
* [ESX Framework](https://www.esx-framework.org/)

---

## Credits

Created and maintained through the **ESX Framework** project and its contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.