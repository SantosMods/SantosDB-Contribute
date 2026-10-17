---
title: ps-dispatch
description: Dispatch and alert system for FiveM built with Svelte and Lua, for QBCore and Qbox.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, qbox, free, github, police, emergency-services
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# ps-dispatch [![](https://badges.5metrics.dev/ps-dispatch/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/ps-dispatch)

Dispatch and alert system for FiveM built with Svelte and Lua, for QBCore and Qbox.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information           |
| ------------- | --------------------- |
| **Name**      | `ps-dispatch`         |
| **Creator**   | Project Sloth & OK1ez |
| **Type**      | Script                |
| **Category**  | Dispatch              |
| **Game**      | FiveM                 |
| **Price**     | Free                  |
| **License**   | GPL-3.0               |
| **Framework** | QBCore, Qbox          |
| **Version**   | `3.0.0`               |
| **Source**    | GitHub                |
| {.dense}      |                       |

---

## Resource Details {.tabset}

### Overview

`ps-dispatch` is a dispatch and alert system for emergency services. Crimes fire alerts, officers respond with a keypress, and the dispatch menu lists open calls with position, responding units, and known suspect and vehicle details.

The README also describes supervisors declaring a major incident and a private plate-check log for each officer.

### Requirements

* `qb-core` or `qbx_core`
* `ox_lib` (locale support requires v3.8.0 or above)
* `PolyZone`
* `lsn-radar` (optional, recommended by the README)

---

## Installation

### Installation Checklist

* [ ] Install `qb-core` or `qbx_core`
* [ ] Install `ox_lib` and `PolyZone`
* [ ] Download `ps-dispatch` from the official repository
* [ ] Build the frontend (`npm install`, then `npm run build` in the `ui` folder)
* [ ] Place `ps-dispatch` in your resources folder
* [ ] Set `Config.Jobs` in `shared/config.lua`
* [ ] Start `ps-dispatch` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure ps-dispatch
```

> The frontend build empties the `html/` folder first. Put files you want served in `ui/public/`.
> {.is-warning}

---

## Configuration

All settings live in `shared/config.lua`. `Config.Jobs` decides which jobs receive alerts. The README gives this default:

```lua
Config.Jobs = { 'police', 'ambulance' }
```

---

## Links

* [GitHub Repository](https://github.com/Project-Sloth/ps-dispatch)
* [Latest Release](https://github.com/Project-Sloth/ps-dispatch/releases/latest)

---

## Credits

Created by **Project Sloth** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.