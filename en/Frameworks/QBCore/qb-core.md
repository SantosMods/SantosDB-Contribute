---
title: qb-core
description: Core FiveM roleplay framework resource for QBCore.
published: true
date: 2026-09-14T01:26:15.532Z
tags: core, framework, qbcore, roleplay
editor: markdown
dateCreated: 2026-09-14T01:26:15.532Z
---

# qb-core [![](https://badges.5metrics.dev/qb-core/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-core)

Core FiveM roleplay framework resource for QBCore.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                     |
| -------------- | --------------------------------------------------------------- |
| **Name**       | `qb-core`                                                       |
| **Creator**    | QBCore Framework                                                |
| **Type**       | Framework                                                       |
| **Category**   | Core Framework                                                  |
| **Game**       | FiveM                                                           |
| **Price**      | Free                                                            |
| **License**    | GPL-3.0                                                         |
| **Framework**  | QBCore                                                          |
| **Repository** | [qbcore-fivem/qb-core](https://github.com/qbcore-fivem/qb-core) |
| {.dense}       |                                                                 |

---

## Resource Details {.tabset}

### Overview

`qb-core` is the core resource for the QBCore FiveM roleplay framework.

The repository contains client, server, shared, locale, and web interface components. It also includes `config.lua`, `fxmanifest.lua`, and `qbcore.sql`.

### Framework Support

| Framework  | Support |
| ---------- | ------- |
| **QBCore** | Native  |
| {.dense}   |         |

### License

The official repository is licensed under GPL-3.0.

---

## Installation

### Installation Checklist

* [ ] Download `qb-core` from the official repository
* [ ] Place `qb-core` in your server resources
* [ ] Review `config.lua`
* [ ] Import the required database schema where applicable
* [ ] Add `qb-core` to your resource startup order
* [ ] Restart the server
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
```

> Other QBCore resources normally depend on `qb-core`, so start it before resources that require it.
> {.is-info}

---

## Configuration

Review `config.lua` and the official QBCore documentation before changing framework settings.

Do not rename the resource unless your dependent resources explicitly support a different name.

---

## Compatibility

| Item              | Information |
| ----------------- | ----------- |
| **Game**          | FiveM       |
| **Framework**     | QBCore      |
| **Resource name** | `qb-core`   |
| {.dense}          |             |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-core)

---

## Before You Install

* [ ] Review the official repository
* [ ] Back up your database before schema changes
* [ ] Confirm dependent QBCore resources use compatible versions
* [ ] Keep the resource name as `qb-core`

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger and ESX/Jérémie N'gadi where applicable.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
