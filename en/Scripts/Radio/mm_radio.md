---
title: mm_radio
description: FiveM radio system using pma-voice, with configurable channels, radio overlays, battery support, and radio jammers.
published: true
date: 2026-09-14T23:54:52.139Z
tags: qbox, radio, script, voice
editor: markdown
dateCreated: 2026-09-14T23:54:52.139Z
---

# mm_radio [![](https://badges.5metrics.dev/mm_radio/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/mm_radio)

FiveM radio system using `pma-voice`, with configurable channels, radio overlays, battery support, and radio jammers.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field                 | Information                                |
| --------------------- | ------------------------------------------ |
| **Name**              | `mm_radio`                                 |
| **Creator**           | SOH69                                      |
| **Type**              | Script                                     |
| **Category**          | Radio                                      |
| **Game**              | FiveM                                      |
| **License**           | GPL-3.0                                    |
| **Framework Support** | QBCore, ESX, Qbox, ND, standalone job list |
| {.dense}              |                                            |

## Resource Details {.tabset}

### Features

The official project documents:

* Radio UI
* Radio submix effect
* Job and gang restricted channels
* Movable and resizable radio UI
* Custom channel display names
* Configurable radio battery
* Radio overlay
* Server-synchronized overlay names
* Placeable radio jammers
* Configurable jammer range
* Frequency exceptions for jammers

### Dependencies

Required dependencies are:

```text
ox_lib
pma-voice
bl_bridge
OneSync
```

The project also documents QBCore, ESX, Qbox, ND, and standalone support for its job list integration.

### Exports

```lua
exports["mm_radio"]:JoinRadio(channel)
exports["mm_radio"]:LeaveRadio()
```

## Installation

> Download an official release unless you intend to build the web source yourself.
> {.is-info}

### Installation Checklist

* [ ] Install `ox_lib`
* [ ] Install `pma-voice`
* [ ] Install `bl_bridge`
* [ ] Enable OneSync
* [ ] Download an official `mm_radio` release
* [ ] Configure your framework and inventory integrations
* [ ] Start dependencies before `mm_radio`
* [ ] Test radio channels, overlay, and jammer behavior

```cfg
ensure ox_lib
ensure pma-voice
ensure bl_bridge
ensure mm_radio
```

### Building From Source

The official repository documents:

```bash
git clone https://github.com/SOH69/mm_radio.git
cd mm_radio/web
pnpm i
pnpm run build
```

## Links

* [Official GitHub Repository](https://github.com/SOH69/mm_radio)
* [Official Releases](https://github.com/SOH69/mm_radio/releases)
* [Official Guide](https://master-mind-store.gitbook.io/dashboard/free-release/radio)

## Credits

Created and maintained by **SOH69** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
