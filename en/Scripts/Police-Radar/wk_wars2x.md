---
title: wk_wars2x
description: Standalone FiveM police radar and plate-reader system inspired by the Stalker DSR 2X.
published: true
date: 2026-09-14T02:18:01.015Z
tags: police, script, standalone, radar
editor: markdown
dateCreated: 2026-09-14T02:18:01.015Z
---

# wk_wars2x [![](https://badges.5metrics.dev/wk_wars2x/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/wk_wars2x)

Standalone FiveM police radar and plate-reader system inspired by the Stalker DSR 2X.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information   |
| ------------- | ------------- |
| **Name**      | `wk_wars2x`   |
| **Project**   | Wraith ARS 2X |
| **Creator**   | WolfKnight98  |
| **Type**      | Script        |
| **Category**  | Police Radar  |
| **Game**      | FiveM         |
| **License**   | MIT           |
| **Framework** | Standalone    |
| {.dense}      |               |

---

## Resource Details {.tabset}

### Overview

Wraith ARS 2X is a police radar system for FiveM.

It tracks traffic using front and rear radar antennas and includes a plate reader.

Documented functionality includes:

* Front and rear radar
* Multiple target-speed tracking
* Operator menu
* Front and rear plate reader
* BOLO plate support
* Developer integration hooks
* Fast-limit locking
* Passenger viewing and controls
* Configurable MPH or KM/H operation
* Sonoran CAD option

### Vehicle Access

The default remote control is intended for the driver of a police vehicle using the `VC_EMERGENCY` vehicle class.

---

## Installation

### Installation Checklist

* [ ] Download the latest official version
* [ ] Place the `wk_wars2x` folder in your resources folder
* [ ] Add the resource to `server.cfg`
* [ ] Review `config.lua`
* [ ] Restart the server
* [ ] Test radar and plate-reader operation in an emergency vehicle

### Resource Order

```cfg
ensure wk_wars2x
```

> The resource checks that its current resource name is `wk_wars2x`.
> {.is-warning}

---

## Configuration

Configuration is stored in:

```text
config.lua
```

Documented settings include:

```lua
CONFIG.allow_fast_limit = true
CONFIG.only_lock_players = false
CONFIG.allow_quick_start_video = true
CONFIG.allow_passenger_view = true
CONFIG.allow_passenger_control = true
CONFIG.use_sonorancad = false
```

Speed display can be configured for:

```text
mph
kmh
```

---

## Default Controls

| Action                 | Default key |
| ---------------------- | ----------- |
| Open remote            | `F5`        |
| Lock/unlock rear plate | `Numpad 6`  |
| Toggle keylock         | `L`         |
| {.dense}               |             |

Keybinds can be changed through resource configuration.

---

## Links

* [Official GitHub Repository](https://github.com/WolfKnight98/wk_wars2x)

---

## Credits

Created by **WolfKnight98** and project contributors.

The project includes additional third-party credits in its source and license notices.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
