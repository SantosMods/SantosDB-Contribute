---
title: bl_bridge
description: Modular FiveM bridge that provides common interfaces across supported frameworks, inventories, targets, menus, notifications, and other systems.
published: true
date: 2026-09-14T23:55:37.167Z
tags: library, qbcore, qbox, framework-bridge
editor: markdown
dateCreated: 2026-09-14T23:55:37.167Z
---

# bl_bridge [![](https://badges.5metrics.dev/bl_bridge/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/bl_bridge)

Modular FiveM bridge that provides common interfaces across supported frameworks, inventories, targets, menus, notifications, and other systems.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field                 | Information           |
| --------------------- | --------------------- |
| **Name**              | `bl_bridge`           |
| **Creator**           | Byte Labs Studio      |
| **Type**              | Library               |
| **Category**          | Framework Bridge      |
| **Game**              | FiveM                 |
| **License**           | GPL-3.0               |
| **Framework Support** | ox, QBCore, ESX, Qbox |
| {.dense}              |                       |

## Resource Details {.tabset}

### Overview

`bl_bridge` is an extendible and modular compatibility bridge for FiveM resources.

It provides common interfaces so resources can support multiple frameworks and ecosystem components without implementing each integration independently.

### Modules

The official configuration documents modules for:

* Framework
* Inventory
* Context menus
* Target systems
* Progress bars
* Radial menus
* Notifications
* Text UI

Modules can be disabled with:

```cfg
setr bl:inventory 'none'
```

### Framework Configuration

Documented framework values are:

```cfg
# 'ox' | 'qb' | 'esx' | 'qbx'
setr bl:framework 'qb'
```

SantosDB uses the canonical discovery tags `qbcore` and `qbox` for the corresponding QBCore and Qbox integrations.

### Imports

Client:

```lua
client_scripts '@bl_bridge/imports/client.lua'
```

Server:

```lua
server_scripts '@bl_bridge/imports/server.lua'
```

## Installation

### Installation Checklist

* [ ] Download `bl_bridge` from Byte Labs Studio
* [ ] Place it in your resources directory
* [ ] Configure the required `bl:*` convars
* [ ] Disable unused modules with `none` where supported
* [ ] Start the bridge before resources that import it
* [ ] Test each selected integration

```cfg
ensure bl_bridge
```

## Links

* [Official GitHub Repository](https://github.com/Byte-Labs-Studio/bl_bridge)

## Credits

Created and maintained by **Byte Labs Studio** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
