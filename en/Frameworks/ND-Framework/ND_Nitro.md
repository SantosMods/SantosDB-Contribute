---
title: ND_Nitro
description: Nitro system for vehicles from the ND Framework organization, used through an ox_inventory item.
published: true
date: 2026-10-16T18:00:00.000Z
tags: script, free, github, vehicles
editor: markdown
dateCreated: 2026-10-16T18:00:00.000Z
---

# ND_Nitro [![](https://badges.5metrics.dev/ND_Nitro/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/ND_Nitro)

Nitro system for vehicles from the ND Framework organization, used through an ox_inventory item.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information             |
| ------------- | ----------------------- |
| **Name**      | `ND_Nitro`              |
| **Creator**   | Andyyy                  |
| **Type**      | Script                  |
| **Category**  | Vehicles                |
| **Game**      | FiveM                   |
| **Price**     | Free                    |
| **License**   | GPL-3.0                 |
| **Framework** | Not specified in README |
| **Version**   | `2.0.1`                 |
| **Source**    | GitHub                  |
| {.dense}      |                         |

---

## Resource Details {.tabset}

### Overview

`ND_Nitro` adds nitro for vehicles. The README shows it being used through an `ox_inventory` item that calls the `ND_Nitro.nos` export.

### Requirements

* `ox_inventory` (listed as the dependency in the README)
* `ox_lib` (loaded by the manifest)

---

## Installation

### Installation Checklist

* [ ] Install `ox_inventory` and `ox_lib`
* [ ] Download `ND_Nitro` from the official repository
* [ ] Place `ND_Nitro` in your resources folder
* [ ] Create the `nos` item in `ox_inventory` as shown in the README
* [ ] Start `ND_Nitro` after its dependencies
* [ ] Check the server console for errors

---

## Item Definition

The README gives this `ox_inventory` item:

```lua
["nos"] = {
    label = "NOS Bottle",
    weight = 2000,
    stack = false,
    close = true,
    client = {
        disable = { move = true, car = true, combat = true },
        usetime = 3500,
        cancel = true,
        export = "ND_Nitro.nos"
    }
},
```

---

## Links

* [GitHub Repository](https://github.com/ND-Framework/ND_Nitro)
* [Latest Release](https://github.com/ND-Framework/ND_Nitro/releases/latest)

---

## Credits

Created by **Andyyy** and the **ND Framework** contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.