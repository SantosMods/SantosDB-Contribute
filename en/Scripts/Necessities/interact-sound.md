---
title: interact-sound
description: FiveM resource for playing sounds through the NUI environment on individual, all, or nearby clients.
published: true
date: 2026-09-14T01:44:03.193Z
tags: audio, script, standalone, nui
editor: markdown
dateCreated: 2026-09-14T01:44:03.193Z
---

# interact-sound [![](https://badges.5metrics.dev/interact-sound/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/interact-sound)

FiveM resource for playing sounds through the NUI environment on individual, all, or nearby clients.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `interact-sound` |
| **Creator**   | plunkettscott    |
| **Type**      | Script           |
| **Category**  | Audio            |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | MIT              |
| **Framework** | Standalone       |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`interact-sound` plays sounds using the FiveM NUI environment.

Sounds can be triggered for:

* One client
* The event source
* All clients
* Clients within a specified distance

### Sound Files

Local sound files are loaded from the resource's NUI sound directory.

The current NUI implementation loads `.ogg` files.

### Events

Documented events include:

```text
InteractSound_SV:PlayOnOne
InteractSound_SV:PlayOnSource
InteractSound_SV:PlayOnAll
InteractSound_SV:PlayWithinDistance
```

Corresponding client events handle playback through NUI.

---

## Installation

### Installation Checklist

* [ ] Download `interact-sound`
* [ ] Place it in your resources folder
* [ ] Add required `.ogg` sound files
* [ ] Add the resource to `server.cfg`
* [ ] Start it before resources that depend on its events
* [ ] Restart the server
* [ ] Test local and distance-based playback

### Resource Order

```cfg
ensure interact-sound
```

---

## Usage

A server resource can trigger the documented sound events to play audio on clients.

Sound volume values are expected within the range documented by the resource.

> Validate any client-controlled sound event usage in your own resources. Do not expose unrestricted server-wide sound playback to untrusted client input.
> {.is-warning}

---

## Compatibility

| Item                  | Information      |
| --------------------- | ---------------- |
| **Game**              | FiveM            |
| **Framework**         | Standalone       |
| **NUI audio**         | Supported        |
| **Distance playback** | Supported        |
| **Resource name**     | `interact-sound` |
| {.dense}              |                  |

---

## Links

* [Official GitHub Repository](https://github.com/plunkettscott/interact-sound)

---

## Before You Install

* [ ] Add the required sound files
* [ ] Check sound file names used by dependent scripts
* [ ] Verify volume settings
* [ ] Test distance-based sounds
* [ ] Start the resource before scripts that use its events

---

## Credits

Created by **plunkettscott** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
