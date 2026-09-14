---
title: luxart-vehicle-control
description: FiveM non-ELS emergency vehicle controller for managing vehicle sirens and emergency lighting.
published: true
date: 2026-09-14T23:54:08.795Z
tags: emergency-services, script, standalone, sirens
editor: markdown
dateCreated: 2026-09-14T23:54:08.795Z
---

# luxart-vehicle-control [![](https://badges.5metrics.dev/lvc/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lvc)

FiveM non-ELS emergency vehicle controller for managing vehicle sirens and emergency lighting.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field                | Information               |
| -------------------- | ------------------------- |
| **Name**             | `luxart-vehicle-control`  |
| **Project**          | Luxart Vehicle Control v3 |
| **Maintainer**       | TrevorBarns               |
| **Original creator** | Lt. Caine                 |
| **Type**             | Script                    |
| **Category**         | Emergency Vehicles        |
| **Game**             | FiveM                     |
| **License**          | GPL-3.0                   |
| **Framework**        | Standalone                |
| {.dense}             |                           |

## Resource Details {.tabset}

### Overview

Luxart Vehicle Control v3 is a siren and non-ELS emergency lighting controller for FiveM.

The project is maintained by TrevorBarns and traces its original implementation to Luxart Vehicle Control by Lt. Caine.

### Configuration

Important configuration files include:

```text
SETTINGS.lua
SIRENS.lua
```

`SETTINGS.lua` controls general LVC behavior.

`SIRENS.lua` contains siren-related configuration.

### Updates

> Back up LVC before updating. Official release notes warn that settings files are not preserved during updates.
> {.is-warning}

Review release notes when upgrading because new releases can require additional settings.

## Installation

### Installation Checklist

* [ ] Download an official LVC release
* [ ] Back up an existing installation before updating
* [ ] Place the resource in your resources directory
* [ ] Configure `SETTINGS.lua`
* [ ] Configure `SIRENS.lua`
* [ ] Add the resource to `server.cfg`
* [ ] Restart the server
* [ ] Test lights, sirens, and configured vehicle profiles

```cfg
ensure luxart-vehicle-control
```

## Links

* [Official GitHub Repository](https://github.com/TrevorBarns/luxart-vehicle-control)
* [Official Releases](https://github.com/TrevorBarns/luxart-vehicle-control/releases)
* [Luxart Engineering](https://www.luxartengineering.com/)

## Credits

**Lt. Caine** created the original Luxart Vehicle Control.

The current project is maintained by **TrevorBarns** and contributors. The project also credits **Faction** for LVC ELS Clicks.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
