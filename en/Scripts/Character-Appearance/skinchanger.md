---
title: skinchanger
description: FiveM skin and character component changer with events for loading and retrieving player appearance data.
published: true
date: 2026-09-14T01:49:58.568Z
tags: appearance, characters, clothing, script
editor: markdown
dateCreated: 2026-09-14T01:49:58.568Z
---

# skinchanger [![](https://badges.5metrics.dev/skinchanger/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/skinchanger)

FiveM skin and character component changer with events for loading and retrieving player appearance data.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information            |
| -------------- | ---------------------- |
| **Name**       | `skinchanger`          |
| **Repository** | `mitlight/skinchanger` |
| **Type**       | Script                 |
| **Category**   | Character Appearance   |
| **Game**       | FiveM                  |
| **Price**      | Free                   |
| **License**    | GPL-3.0                |
| {.dense}       |                        |

---

## Resource Details {.tabset}

### Overview

`skinchanger` provides events for loading player models, applying skin data, changing individual appearance components, and retrieving the current skin.

The repository is a fork of the ESX `skinchanger` project.

### License

The repository includes the GNU General Public License version 3.

Its license notice credits **Jérémie N'gadi** for the original `skinchanger` project.

---

## Installation

### Installation Checklist

* [ ] Download `skinchanger`
* [ ] Place it in your resources folder
* [ ] Add it to `server.cfg`
* [ ] Start the resource
* [ ] Test skin loading with your appearance integration

### Resource Order

```cfg
start skinchanger
```

---

## Usage

The resource documents events including:

```lua
TriggerEvent('skinchanger:loadDefaultModel', isMale)
TriggerEvent('skinchanger:loadSkin', skin)
```

Retrieve component data:

```lua
TriggerEvent('skinchanger:getData', function(components, maxVals)
    print(json.encode(components))
    print(json.encode(maxVals))
end)
```

Retrieve the current skin:

```lua
TriggerEvent('skinchanger:getSkin', function(skin)
    print(json.encode(skin))
end)
```

---

## Links

* [Official repository](https://github.com/mitlight/skinchanger)

---

## Credits

This repository is maintained under **mitlight**.

The included license and project notice credit **Jérémie N'gadi** as the original `skinchanger` author.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
