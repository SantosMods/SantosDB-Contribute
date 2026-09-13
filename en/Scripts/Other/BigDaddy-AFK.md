---
title: BigDaddy-AFK
description: Monitors keyboard, mouse, and controller activity to remove inactive players while providing events that temporarily suspend AFK checks.
published: true
date: 2026-09-13T15:37:35.531Z
tags: qbcore, qbox, script, afk
editor: markdown
dateCreated: 2026-09-13T15:37:35.531Z
---

# AFK [![](https://badges.5metrics.dev/BigDaddy-AFK/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-AFK)

AFK monitors keyboard, mouse, and controller activity and removes players after a configurable period of inactivity.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information               |
| ------------------- | ------------------------- |
| **Name**            | `AFK`                     |
| **Resource Folder** | `BigDaddy-AFK`            |
| **Creator**         | Big Daddy Scripts         |
| **Game**            | FiveM                     |
| **Type**            | Script                    |
| **Category**        | Player Management         |
| **Version**         | `v1.0.1`                  |
| **Price**           | $3.00 USD                 |
| **Dependencies**    | None                      |
| **QBCore / Qbox**   | ✅ Integrated and verified |
| **ESX**             | ✅ Integrated and verified |
| **Runtime**         | CFX Mono V2               |
| {.dense}            |                           |

Unlike AFK systems based only on player position, AFK monitors actual keyboard, mouse, and controller input.

---

## Resource Details {.tabset}

### Overview

AFK automatically monitors player activity and removes inactive players after the configured timeout.

The script provides events that other resources can trigger to suspend AFK monitoring during activities such as character creation or character selection.

### Features

* Monitors keyboard input
* Monitors mouse input
* Monitors controller input
* Does not determine AFK status from player position
* Configurable inactivity timeout
* Configurable activity check interval
* Configurable controller deadzone
* Configurable warning and kick messages
* Suspend and resume client events

### Framework Support

| Framework       | Status                     |
| --------------- | -------------------------- |
| **Stand-Alone** | Supported                  |
| **QBCore**      | ✅ Implemented and verified |
| **Qbox**        | ✅ Implemented and verified |
| **ESX**         | ✅ Implemented and verified |
| {.dense}        |                            |

Big Daddy Scripts defines **✅** as implemented with the framework and verified working.

---

## Installation

### Installation Checklist

* [ ] Remove conflicting AFK resources.
* [ ] Download AFK from Big Daddy Scripts.
* [ ] Extract `BigDaddy-AFK` into your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.
* [ ] Check the consoles for errors.

```cfg
start BigDaddy-AFK
```

> Do not rename `BigDaddy-AFK`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

> Remove other AFK scripts such as `qbx-afk`. Running multiple AFK systems at the same time can cause them to compete with each other.
> {.is-danger}

---

## Configuration

AFK uses `settings.ini`.

| Setting            | Default | Description                                       |
| ------------------ | ------- | ------------------------------------------------- |
| `key1`             | `none`  | Big Daddy Scripts product key                     |
| `AfkTimeoutMin`    | `15`    | Minutes of inactivity before the player is kicked |
| `CheckIntervalMs`  | `1000`  | Milliseconds between activity checks              |
| `AxisDeadzone`     | `0.05`  | Controller axis deadzone allowance                |
| `KickMessage`      | blank   | Message shown when the player is kicked           |
| `WarnMessage`      | blank   | Warning shown to the player                       |
| `CountdownMessage` | blank   | Message shown during the countdown before removal |
| {.dense}           |         |                                                   |

---

## Client Events

Use the provided events when another resource needs to temporarily prevent AFK removal.

### Suspend Monitoring

```lua
TriggerEvent("BigDaddy-AFK:Suspend")
```

This stops AFK monitoring for the current client.

### Resume Monitoring

```lua
TriggerEvent("BigDaddy-AFK:Resume")
```

This resumes AFK monitoring for the current client.

These events are intended for situations such as character creation and character selection where a player may legitimately remain still.

---

## Usage

No player command is required.

AFK automatically monitors activity and removes inactive players according to the configured timeout.

---

## Compatibility

The current Big Daddy Scripts compatibility table marks QBCore/Qbox and ESX with **✅**, indicating framework implementation and verified compatibility.

The script uses CFX Mono V2. Big Daddy Scripts states that this runtime requires game build `3095+` and that they test on build `3095`.

---

## Official Links

* [AFK Product Page](https://bigdaddyscripts.com/Products/View/3184/AFK)
* [AFK Documentation](https://wiki.bigdaddyscripts.com/Documentation/AFK/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
