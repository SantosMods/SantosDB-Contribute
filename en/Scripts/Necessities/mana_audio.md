---
title: mana_audio
description: FiveM API for playing native audio globally, from entities, or from world coordinates.
published: true
date: 2026-09-14T02:18:49.121Z
tags: audio, developer-tool, library, standalone
editor: markdown
dateCreated: 2026-09-14T02:18:49.121Z
---

# mana_audio [![](https://badges.5metrics.dev/mana_audio/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/mana_audio)

FiveM API for playing native audio globally, from entities, or from world coordinates.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information  |
| ------------- | ------------ |
| **Name**      | `mana_audio` |
| **Creator**   | Manason      |
| **Type**      | Library      |
| **Category**  | Audio        |
| **Game**      | FiveM        |
| **License**   | GPL-3.0      |
| **Framework** | Standalone   |
| {.dense}      |              |

---

## Resource Details {.tabset}

### Overview

`mana_audio` provides client and server exports for playing native game audio.

Audio can be played:

* Without a 3D world position
* From an entity
* From coordinates

The server API can send sounds to clients.

### Limitations

The official project states that:

* Stopping audio before it finishes is not supported
* Looping audio is not supported

---

## Installation

### Installation Checklist

* [ ] Download `mana_audio`
* [ ] Place it in your resources folder
* [ ] Add it to `server.cfg`
* [ ] Start it before resources using its exports
* [ ] Test the native audio banks and references used by your script

### Resource Order

```cfg
ensure mana_audio
```

---

## Usage {.tabset}

### Client

Play non-positional audio:

```lua
exports.mana_audio:PlaySound({
    audioBank = 'myAudioBank',
    audioName = {'myAudioName1', 'myAudioName2'},
    audioRef = 'myAudioRef'
})
```

Play audio from an entity:

```lua
exports.mana_audio:PlaySoundFromEntity({
    audioBank = 'myAudioBank',
    audioName = {'myAudioName1', 'myAudioName2'},
    audioRef = 'myAudioRef',
    entity = PlayerPedId()
})
```

Play audio from coordinates:

```lua
exports.mana_audio:PlaySoundFromCoords({
    audioBank = 'myAudioBank',
    audioName = {'myAudioName1', 'myAudioName2'},
    audioRef = 'myAudioRef',
    coords = vec3(0, 0, 0),
    range = 10
})
```

### Server

The server API provides corresponding `PlaySound`, `PlaySoundFromEntity`, and `PlaySoundFromCoords` exports.

A server `PlaySound` call can target a specific client or `-1` for all clients.

---

## Links

* [Official GitHub Repository](https://github.com/Manason/mana_audio)

---

## Credits

Created by **Manason**.

The project specifically thanks **PrinceAlbert**, **Demi-Automatic**, **ChatDisabled**, **Joe Szymkowicz**, and **Zoo**.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
