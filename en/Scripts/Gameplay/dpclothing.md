---
title: dpclothing
description: FiveM clothing utility for toggling and changing character clothing components and variations.
published: true
date: 2026-09-14T23:51:46.616Z
tags: appearance, characters, clothing, script
editor: markdown
dateCreated: 2026-09-14T23:51:46.616Z
---

# dpclothing [![](https://badges.5metrics.dev/dpclothing/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/dpclothing)

FiveM clothing utility for toggling and changing character clothing components and variations.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field                           | Information            |
| ------------------------------- | ---------------------- |
| **Name**                        | `dpclothing`           |
| **Project**                     | dpClothing+            |
| **Repository**                  | `andristum/dpclothing` |
| **Original author in manifest** | `dullpear`             |
| **Type**                        | Script                 |
| **Category**                    | Clothing               |
| **Game**                        | FiveM                  |
| **Version in manifest**         | `1.0.3`                |
| **License**                     | Unknown                |
| {.dense}                        |                        |

## Resource Details {.tabset}

### Overview

`dpclothing` provides clothing variations and toggles for FiveM characters.

The resource contains separate client files for configuration, clothing logic, variations, GUI functionality, and locales.

### Files

The current manifest loads:

```text
Client/Functions.lua
Locale/*.lua
Client/Config.lua
Client/Variations.lua
Client/Clothing.lua
Client/GUI.lua
```

The manifest identifies `Client/Variations.lua` as the primary location for changing clothing variations.

## Installation

### Installation Checklist

* [ ] Download `dpclothing` from the official repository
* [ ] Keep the resource folder named `dpclothing`
* [ ] Place it in your resources directory
* [ ] Review `Client/Config.lua`
* [ ] Review `Client/Variations.lua`
* [ ] Add the resource to `server.cfg`
* [ ] Test configured clothing toggles

```cfg
ensure dpclothing
```

## Configuration

Review:

```text
Client/Config.lua
Client/Variations.lua
```

Preserve the component and variation structure expected by the resource when customizing clothing.

## Links

* [Official GitHub Repository](https://github.com/andristum/dpclothing)
* [Official Cfx.re Release](https://forum.cfx.re/t/dpclothing-1-0-0-clothing-variations-and-toggles-gloves-vest-top-hair-bag-and-more/1326317)

## Credits

The repository is hosted under **andristum**.

The resource manifest credits **dullpear** as the author.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
