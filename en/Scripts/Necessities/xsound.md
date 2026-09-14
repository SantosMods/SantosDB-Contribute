---
title: xsound
description: FiveM audio library for playing and controlling URL-based and positional sounds.
published: true
date: 2026-09-14T01:41:34.397Z
tags: script, standalone, audio, sound
editor: markdown
dateCreated: 2026-09-14T01:41:34.397Z
---

# xsound [![](https://badges.5metrics.dev/xsound/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/xsound)

FiveM audio library for playing and controlling URL-based and positional sounds.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `xsound`         |
| **Creator**   | Xogy             |
| **Type**      | Script / Library |
| **Category**  | Audio            |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | MIT              |
| **Framework** | Standalone       |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`xsound` is an audio library for FiveM.

It can play sounds globally or at world coordinates and provides functions for controlling active sounds.

### Playback

Documented client functions include:

```lua
PlayUrl(name, URL, volume, loop, options)
PlayUrlPos(name, url, volume, Vector3, loop, options)
```

`PlayUrl` plays a URL without positional audio.

`PlayUrlPos` plays a sound at specified coordinates.

### Sound Control

The API provides functions for manipulating active sounds, including changing their position and other playback properties.

### interact-sound Compatibility

`xsound` includes an `interact-sound` emulator.

To use it, move the required sounds from `interact-sound` into:

```text
xsound/html/sounds
```

and enable the corresponding emulator configuration.

---

## Installation

### Installation Checklist

* [ ] Download `xsound`
* [ ] Place it in your resources folder
* [ ] Add it to your startup configuration
* [ ] Configure any required sound files
* [ ] Configure `interact-sound` emulation only if required
* [ ] Restart the server
* [ ] Test local and positional audio

### Resource Order

```cfg
ensure xsound
```

---

## Usage

Example playback functions:

```lua
PlayUrl(name, URL, volume)
PlayUrlPos(name, URL, volume, vector3(x, y, z))
```

Use the official repository for the complete API and current parameter definitions.

---

## Compatibility

| Item                             | Information |
| -------------------------------- | ----------- |
| **Game**                         | FiveM       |
| **Framework**                    | Standalone  |
| **Positional audio**             | Supported   |
| **interact-sound API emulation** | Available   |
| **Resource name**                | `xsound`    |
| {.dense}                         |             |

---

## Links

* [Official GitHub Repository](https://github.com/Xogy/xsound)

---

## Before You Install

* [ ] Review the current API
* [ ] Check resources that depend on `interact-sound`
* [ ] Move local sound files when using `interact-sound` emulation
* [ ] Test URL accessibility for remotely hosted audio
* [ ] Test positional sound distances

---

## Credits

Created by **Xogy** and project contributors.

The project credits **plunkettscott** and `interact-sound` for its sound API work.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
