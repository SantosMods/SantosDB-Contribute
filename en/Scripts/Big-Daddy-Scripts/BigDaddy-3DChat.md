---
title: BigDaddy-3DChat
description: Displays local chat messages as 3D bubbles above players, with configurable distance, duration, and message length.
published: true
date: 2026-09-13T15:30:49.088Z
tags: proximity-chat, qbcore, qbox, script
editor: markdown
dateCreated: 2026-09-13T15:29:04.238Z
---

# 3DChat [![](https://badges.5metrics.dev/BigDaddy-3DChat/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-3DChat)

3DChat displays local chat messages as 3D chat bubbles above players instead of only displaying them in the standard chat box.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information                          |
| ------------------- | ------------------------------------ |
| **Name**            | `3DChat`                             |
| **Resource Folder** | `BigDaddy-3DChat`                    |
| **Creator**         | Big Daddy Scripts                    |
| **Game**            | FiveM                                |
| **Type**            | Script                               |
| **Category**        | Chat                                 |
| **Version**         | `v1.3.1`                             |
| **Price**           | $10.00 USD                           |
| **QBCore**          | Compatible, not framework integrated |
| **Qbox**            | Compatible, not framework integrated |
| **ESX**             | Compatibility warning                |
| **BigDaddy-Chat**   | Supported with `v1.13` and above     |
| **License**         | Proprietary / product key required   |
| {.dense}            |                                      |

The official compatibility matrix marks QBCore and Qbox with **✔**, meaning 3DChat is verified as a Stand-Alone script that should work with those frameworks but is not integrated with them.

ESX is marked **⚠️**, meaning it should work, but compatibility issues may arise.

> 3DChat does not currently display framework character names.
> {.is-warning}

---

## Resource Details {.tabset}

### Overview

3DChat replaces the usual presentation of local messages with chat bubbles positioned above players.

The script adjusts bubble positioning for players inside vehicles. The offset changes based on the occupied seat and supports vehicles including cars, aircraft, and motorcycles.

Longer messages remain visible longer to provide additional reading time.

When messages are submitted close together, the script queues their display rather than immediately placing both bubbles over each other.

### Features

* Displays local proximity messages as 3D chat bubbles
* Supports configurable maximum chat distance
* Supports configurable display duration
* Supports configurable maximum message length
* Adjusts bubbles for occupied vehicle seats
* Provides local `/me` and `/do` commands
* Provides alternate `/3dme` and `/3ddo` commands
* Supports LEO and medical message types
* Can duplicate messages into the standard chat box
* Works with `BigDaddy-Chat` `v1.13` and newer

### Framework Support

| Framework       | Compatibility            | Integration             |
| --------------- | ------------------------ | ----------------------- |
| **Stand-Alone** | Supported                | Native operation        |
| **QBCore**      | ✔ Verified working       | No                      |
| **Qbox**        | ✔ Verified working       | No                      |
| **ESX**         | ⚠️ Compatibility warning | No verified integration |
| {.dense}        |                          |                         |

> A **✔** in Big Daddy Scripts' compatibility matrix does not indicate framework integration. It means the Stand-Alone resource has been verified to work without a known blocking issue.
> {.is-info}

---

## Requirements

3DChat uses the resource folder:

```text
BigDaddy-3DChat
```

A Big Daddy Scripts product key must be added to `settings.ini`.

> Do not rename the `BigDaddy-3DChat` resource folder. The official documentation states that changing the folder name will prevent the resource from functioning correctly.
> {.is-danger}

### Game Build

The current Big Daddy Scripts product page states that the script uses the CFX Mono V2 runtime.

Game build `2944` is not supported by this runtime. Big Daddy Scripts requires build `3095` or newer and recommends `3095`, which is the build they test against.

Console warnings related to the CFX Mono V2 runtime may appear because the runtime is listed as beta.

---

## Installation

### Installation Checklist

* [ ] Purchase and download 3DChat from Big Daddy Scripts.
* [ ] Extract the downloaded ZIP.
* [ ] Place `BigDaddy-3DChat` inside your server resources folder.
* [ ] Keep the `BigDaddy-3DChat` folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.
* [ ] Check the client and server consoles.

### Resource Order

Add the following to `server.cfg`:

```cfg
start BigDaddy-3DChat
```

> BigDaddy-Chat is **not required** to use 3DChat.
> {.is-info}

---

## Configuration

3DChat uses `settings.ini` for its documented configuration.

| Setting               | Default | Purpose                                                  |
| --------------------- | ------: | -------------------------------------------------------- |
| `key1`                |  `none` | Big Daddy Scripts product key                            |
| `offsetX`             |   `-.2` | Adjusts the bubble position on the X axis                |
| `offsetY`             |     `0` | Adjusts the bubble position on the Y axis                |
| `offsetZ`             |   `1.3` | Adjusts the bubble position on the Z axis                |
| `displayTime`         |  `6400` | Base bubble display time in milliseconds                 |
| `maxCharacters`       |   `750` | Maximum characters allowed in one message                |
| `addMessagesToSkybox` | `false` | Duplicates messages to the regular chat box when enabled |
| `maxChatDistance`     |    `20` | Maximum bubble viewing distance in meters                |
| {.dense}              |         |                                                          |

Long messages can remain visible beyond the configured base `displayTime`.

Messages exceeding `maxCharacters` are truncated.

---

## Commands

All documented 3DChat commands are local chat commands.

| Command  | Function                                                |
| -------- | ------------------------------------------------------- |
| `/me`    | Displays **ME** before the message                      |
| `/3dme`  | Alternate **ME** command for avoiding command conflicts |
| `/do`    | Displays **DO** before the message                      |
| `/3ddo`  | Alternate **DO** command for avoiding command conflicts |
| `/leo`   | Displays **LEO** before the message                     |
| `/med`   | Displays **MED** before the message                     |
| {.dense} |                                                         |

The `/3dme` and `/3ddo` alternatives allow 3DChat to be used alongside chat resources that already register `/me` or `/do`.

---

## BigDaddy-Chat Integration

3DChat works with `BigDaddy-Chat` `v1.13` and newer.

When using both resources, configure the corresponding BigDaddy-Chat setting:

```ini
supressLocalCommands=true
```

This allows 3DChat to handle the local commands instead of BigDaddy-Chat overriding them.

> `supressLocalCommands` uses the spelling shown in the official Big Daddy Scripts 3DChat documentation.
> {.is-info}

---

## Compatibility Notes

### Framework Character Names

3DChat does not currently display framework character names according to the official documentation.

### Invisible Players

An update added handling for invisible or noclipped players. When a player is invisible when submitting a message, the message is sent to regular chat instead of displaying as a bubble.

### Multiple Messages

Messages submitted close together are queued so the first message can finish displaying before the next one appears.

The creator notes that more than two messages entered in rapid succession may display out of order.

---

## Recent Updates

| Version  | Date              | Changes                                                                             |
| -------- | ----------------- | ----------------------------------------------------------------------------------- |
| `v1.3.1` | July 31, 2026     | Removed a broken CFX native used for HTTP calls to address desync timeouts          |
| `v1.2.2` | April 28, 2026    | Updated licensing with the latest timeout fix                                       |
| `v1.2.1` | April 13, 2026    | Added a startup procedure for slower connections                                    |
| `v1.2.0` | April 7, 2025     | Added configurable chat distance, changed distance calculation, and added a ZAP fix |
| `v1.11`  | July 12, 2024     | Added `/3dme` and `/3ddo` alternate commands                                        |
| `v1.1`   | November 14, 2023 | Added handling for invisible or noclipped players                                   |
| {.dense} |                   |                                                                                     |

---

## Before You Install

* [ ] Confirm your server uses game build `3095` or newer.
* [ ] Keep the folder named `BigDaddy-3DChat`.
* [ ] Obtain your valid Big Daddy Scripts product key.
* [ ] Configure `settings.ini`.
* [ ] Check framework compatibility.
* [ ] Configure `supressLocalCommands` if you also use BigDaddy-Chat.
* [ ] Expect CFX Mono V2 beta warnings in the client and server consoles.

---

## Official Links

* [3DChat Product Page](https://bigdaddyscripts.com/Products/View/2287/3DChat)
* [3DChat Documentation](https://wiki.bigdaddyscripts.com/Documentation/3DChat/)
* [Big Daddy Scripts Compatibility](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
