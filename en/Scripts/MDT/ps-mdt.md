---
title: ps-mdt
description: FiveM law-enforcement MDT for QBCore and Qbox through the ps_lib framework abstraction layer.
published: true
date: 2026-09-14T02:14:58.197Z
tags: police, qbcore, qbox, script
editor: markdown
dateCreated: 2026-09-14T02:14:58.197Z
---

# ps-mdt [![](https://badges.5metrics.dev/ps-mdt/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/ps-mdt)

FiveM law-enforcement MDT for QBCore and Qbox through the `ps_lib` framework abstraction layer.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information     |
| --------------------- | --------------- |
| **Name**              | `ps-mdt`        |
| **Creator**           | Project Sloth   |
| **Type**              | Script          |
| **Category**          | Police MDT      |
| **Game**              | FiveM           |
| **License**           | CC BY-NC-SA 4.0 |
| **Framework Support** | QBCore, Qbox    |
| {.dense}              |                 |

---

## Resource Details {.tabset}

### Overview

`ps-mdt` v3 is an in-game law-enforcement computer built with Svelte 5 and Lua.

Documented functionality includes:

* Citizen lookup
* Reports
* Cases
* Evidence
* Warrants
* BOLOs
* Vehicle lookup
* Weapon lookup
* Security cameras
* Bodycam feeds
* Dispatch
* Department management

Access is permission based.

### Requirements

Required dependencies:

* `ps_lib`
* `oxmysql`
* `ox_lib`
* `screenshot-basic`

Optional integrations recommended by the project:

* `ps-dispatch`
* `ps-multijob`

### Framework Support

`ps-mdt` uses `ps_lib` as its framework abstraction layer.

The current project documents support for:

* QBCore
* Qbox

---

## Installation

> `ps-mdt` v3 is not backwards compatible with `ps-mdt` v1.
> {.is-warning}

### Installation Checklist

* [ ] Install `ps_lib`
* [ ] Install `oxmysql`
* [ ] Install `ox_lib`
* [ ] Install `screenshot-basic`
* [ ] Download `ps-mdt`
* [ ] Configure required jobs
* [ ] Import the framework SQL
* [ ] Configure optional FiveManage API keys
* [ ] Build the frontend if your download does not include `web/dist`
* [ ] Start `ps-mdt` after its dependencies

### Resource Order

```cfg
ensure ps_lib
ensure oxmysql
ensure ox_lib
ensure screenshot-basic
ensure ps-mdt
```

### Database

For QBCore, the current README instructs you to run:

```text
sql/qbcore.sql
```

against the FiveM database.

---

## Configuration

Optional FiveManage integrations use:

```cfg
set ps_mdt_fivemanage_key_images "YOUR_IMAGES_API_KEY_HERE"
set ps_mdt_fivemanage_key_logs "YOUR_LOGS_API_KEY_HERE"
```

The image key is used for image uploads.

The log key forwards audit activity to FiveManage Logs.

Do not publish private API keys.

---

## Usage

Open the MDT with:

```text
/mdt
```

The documented default key is:

```text
F11
```

---

## Links

* [Official GitHub Repository](https://github.com/Project-Sloth/ps-mdt)

---

## Credits

Created and maintained by **Project Sloth** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
