---
title: MugShotBase64
description: Standalone FiveM resource that converts ped mugshots to Base64 strings for storage or use by other scripts.
published: true
date: 2026-09-14T01:44:43.473Z
tags: developer-tool, script, standalone, mugshot
editor: markdown
dateCreated: 2026-09-14T01:44:43.473Z
---

# MugShotBase64 [![](https://badges.5metrics.dev/MugShotBase64/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/MugShotBase64)

Standalone FiveM resource that converts ped mugshots to Base64 strings for storage or use by other scripts.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information     |
| ------------- | --------------- |
| **Name**      | `MugShotBase64` |
| **Creator**   | BaziForYou      |
| **Type**      | Script          |
| **Category**  | Mugshot Utility |
| **Game**      | FiveM           |
| **Price**     | Free            |
| **License**   | MIT             |
| **Framework** | Standalone      |
| {.dense}      |                 |

---

## Resource Details {.tabset}

### Overview

`MugShotBase64` converts a ped mugshot into a Base64 string.

The resulting string can be stored as text in systems such as JSON, SQL, or text files without uploading the mugshot to an external image host.

The resource can generate a mugshot from a specified ped rather than only the local player's ped.

### Requirements

The project is standalone and does not document a framework dependency.

### Export

The documented client export is:

```text
GetMugShotBase64
```

It accepts a ped handle and transparency boolean and returns a string.

---

## Installation

### Installation Checklist

* [ ] Download `MugShotBase64`
* [ ] Place `MugShotBase64` in your resources folder
* [ ] Add it to `server.cfg`
* [ ] Start it before resources that use its export
* [ ] Restart the server
* [ ] Test Base64 mugshot generation

### Resource Order

```cfg
start MugShotBase64
```

---

## Usage

Example from the official documentation:

```lua
local MugShot = exports["MugShotBase64"]:GetMugShotBase64(PlayerPedId(), true)
```

The export returns the mugshot as a Base64 string.

---

## Compatibility

| Item              | Information     |
| ----------------- | --------------- |
| **Game**          | FiveM           |
| **Framework**     | Standalone      |
| **Output**        | Base64 string   |
| **Ped selection** | Supported       |
| **Resource name** | `MugShotBase64` |
| {.dense}          |                 |

---

## Links

* [Official GitHub Repository](https://github.com/BaziForYou/MugShotBase64)

---

## Before You Install

* [ ] Keep the resource name as `MugShotBase64`
* [ ] Start it before dependent scripts
* [ ] Check database field sizes before storing Base64 images
* [ ] Test transparency settings required by your integration

---

## Credits

Created by **BaziForYou** and project contributors.

The project also credits **codegrepper**.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
