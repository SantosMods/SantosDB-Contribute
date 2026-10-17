---
title: EUP-Menu
description: EUP uniform menu for FiveM with a player menu, an admin menu for saving uniforms, and ACE or Discord role permissions.
published: true
date: 2026-10-16T18:00:00.000Z
tags: script, free, github, eup
editor: markdown
dateCreated: 2026-10-16T18:00:00.000Z
---

# EUP-Menu [![](https://badges.5metrics.dev/EUP-Menu/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/EUP-Menu)

EUP uniform menu for FiveM with a player menu, an admin menu for saving uniforms, and ACE or Discord role permissions.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field        | Information |
| ------------ | ----------- |
| **Name**     | `EUP-Menu`  |
| **Creator**  | Copeman     |
| **Type**     | Script      |
| **Category** | EUP Menu    |
| **Game**     | FiveM       |
| **Price**    | Free        |
| **License**  | MIT         |
| **Version**  | `1.0.0`     |
| **Source**   | GitHub      |
| {.dense}     |             |

---

## Resource Details {.tabset}

### Overview

`EUP-Menu` has two menus. `/eup` lets players apply saved uniforms. `/eupadmin` lets admins create menus and submenus and save the clothing they are wearing as a uniform. Data is stored in `outfits.json`.

### Requirements

* `RageUI`
* `ox_lib`
* A Discord bot token and guild ID (only for Discord role permissions)

### Features

* Player menu (`/eup`) and admin menu (`/eupadmin`)
* Menus and submenus, for example `Police/Patrol`
* Permissions by ACE or up to 4 Discord roles
* Persistent storage in `outfits.json`

---

## Installation

### Installation Checklist

* [ ] Install `RageUI` and `ox_lib`
* [ ] Download `EUP-Menu` from the official repository
* [ ] Place it in your resources folder
* [ ] Edit `config.lua` for permissions
* [ ] Add the resources to `server.cfg`
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure RageUI
ensure ox_lib
ensure EUP-Menu
```

> Do not publish the Discord `BotToken` from `config.lua`. The README says Discord permissions need a bot with the Server Members Intent enabled.
> {.is-warning}

---

## Links

* [GitHub Repository](https://github.com/Copeman-1/EUP-Menu)

---

## Credits

Created by **Copeman**.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.