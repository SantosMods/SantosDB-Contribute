---
title: illenium-appearance
description: Character appearance and clothing resource supporting qb-core, ESX, and ox_core.
published: true
date: 2026-09-14T01:43:22.125Z
tags: appearance, esx, qbcore, script
editor: markdown
dateCreated: 2026-09-14T01:43:22.125Z
---

# illenium-appearance [![](https://badges.5metrics.dev/illenium-appearance/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/illenium-appearance)

Character appearance and clothing resource supporting qb-core, ESX, and ox_core.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information           |
| -------------- | --------------------- |
| **Name**       | `illenium-appearance` |
| **Creator**    | iLLeniumStudios       |
| **Type**       | Script                |
| **Category**   | Character Appearance  |
| **Game**       | FiveM                 |
| **Price**      | Free                  |
| **License**    | MIT                   |
| **Frameworks** | qb-core, ESX, ox_core |
| {.dense}       |                       |

---

## Resource Details {.tabset}

### Overview

`illenium-appearance` is a replacement clothing and character appearance resource for multiple FiveM frameworks.

Documented features include:

* Player outfits
* Job and gang clothing rooms
* Job and gang restricted stores
* Tattoos
* Hair textures
* PolyZone support
* Plastic surgeons
* `qb-target` support
* Skin migration
* Player-specific outfit locations
* Component, prop, and ped restrictions
* Persistent job and gang clothing
* Themes
* Clothing-as-items support

### Framework Support

| Framework   | Support      |
| ----------- | ------------ |
| **qb-core** | Supported    |
| **ESX**     | Supported    |
| **ox_core** | Experimental |
| {.dense}    |              |

### Dependencies

`ox_lib` is required.

Framework-specific dependencies are:

* `qb-core` for qb-core servers
* `es_extended` for ESX servers
* `ox_core` for ox_core servers

`qb-target` is optional for qb-core installations.

---

## Installation

> Do not install the `main` branch for a production server. The creator explicitly instructs users to install the latest release.
> {.is-warning}

### Installation Checklist

* [ ] Download the latest official release
* [ ] Install `ox_lib`
* [ ] Install your selected framework
* [ ] Install optional `qb-target` integration if required
* [ ] Follow the framework-specific installation documentation
* [ ] Configure appearance locations and options
* [ ] Start dependencies before `illenium-appearance`
* [ ] Restart the server
* [ ] Test character creation and clothing

### Resource Order

Example:

```cfg
ensure ox_lib
ensure illenium-appearance
```

Your framework must also start in the order required by its official installation instructions.

---

## Usage

Documented commands include:

```text
/pedmenu
/reloadskin
```

`/pedmenu` is configurable.

---

## Migration

The resource documents migration support for:

* `qb-clothing`
* Older `fivem-appearance`
* `esx_skin`

Follow the official migration documentation for your existing appearance system.

> Back up your database before running appearance or skin migrations.
> {.is-danger}

---

## Compatibility

| Item              | Information           |
| ----------------- | --------------------- |
| **Game**          | FiveM                 |
| **qb-core**       | Supported             |
| **ESX**           | Supported             |
| **ox_core**       | Experimental          |
| **ox_lib**        | Required              |
| **qb-target**     | Optional for qb-core  |
| **Resource name** | `illenium-appearance` |
| {.dense}          |                       |

---

## Links

* [Official GitHub Repository](https://github.com/iLLeniumStudios/illenium-appearance)
* [Official Releases](https://github.com/iLLeniumStudios/illenium-appearance/releases/latest)
* [Official Documentation](https://docs.illenium.dev)

---

## Before You Install

* [ ] Use the latest release, not the `main` branch
* [ ] Install `ox_lib`
* [ ] Select the correct framework configuration
* [ ] Back up existing appearance data before migration
* [ ] Review optional `qb-target` support
* [ ] Test clothing, tattoos, outfits, and character loading

---

## Credits

Created and maintained by **iLLeniumStudios** and project contributors.

The project credits the original `fivem-appearance` by **pedr0fontoura**, tattoo support work by **franfdezmorales**, and the previously maintained QBCore fork by **mirrox1337**.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
