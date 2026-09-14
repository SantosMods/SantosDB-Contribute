---
title: pma-voice
description: FiveM and RedM voice system built around the internal Mumble server.
published: true
date: 2026-09-14T01:39:39.074Z
tags: script, standalone, voice, mumble
editor: markdown
dateCreated: 2026-09-14T01:39:39.074Z
---

# pma-voice [![](https://badges.5metrics.dev/pma-voice/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/pma-voice)

FiveM and RedM voice system built around the internal Mumble server.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information   |
| -------------- | ------------- |
| **Name**       | `pma-voice`   |
| **Creator**    | AvarianKnight |
| **Type**       | Script        |
| **Category**   | Voice         |
| **Games**      | FiveM, RedM   |
| **Price**      | Free          |
| **License**    | Unknown       |
| **Framework**  | Standalone    |
| **Dependency** | OneSync       |
| {.dense}       |               |

---

## Resource Details {.tabset}

### Overview

`pma-voice` is a VOIP resource that uses the internal Mumble server provided by FiveM and RedM.

The resource provides proximity voice, radio, call, submix, and voice UI functionality.

### Requirements

The current `fxmanifest.lua` declares:

```text
/onesync
```

as a dependency.

### Compatibility

`pma-voice` is not compatible with another active voice system.

Disable other voice implementations, including vMenu voice chat, when using `pma-voice`.

Do not override these natives from other resources:

```text
NetworkSetTalkerProximity
MumbleSetTalkerProximity
MumbleSetAudioInputDistance
MumbleSetAudioOutputDistance
NetworkSetVoiceActive
```

---

## Installation

### Installation Checklist

* [ ] Enable OneSync
* [ ] Download `pma-voice`
* [ ] Place `pma-voice` in your resources folder
* [ ] Remove or disable conflicting voice systems
* [ ] Configure voice convars
* [ ] Add `pma-voice` to `server.cfg`
* [ ] Restart the server
* [ ] Test proximity, radio, and call audio

### Resource Order

```cfg
ensure pma-voice
```

---

## Configuration

`pma-voice` uses convars for configuration.

Current options include settings for:

* Native audio
* 2D audio
* Voice UI
* Proximity cycling
* Radio volume
* Call volume
* Radios
* Calls
* Submix
* Radio animation
* Radio key
* External Mumble servers
* Debug mode

> The current branch contains breaking configuration changes. `voice_defaultPhoneVolume` was replaced by `voice_defaultCallVolume`, and `voice_enablePhones` was replaced by `voice_enableCalls`.
> {.is-warning}

The `phone` player state was also replaced by `call`.

---

## Compatibility

| Item                    | Information                 |
| ----------------------- | --------------------------- |
| **FiveM**               | Supported                   |
| **RedM**                | Supported                   |
| **OneSync**             | Required                    |
| **Other voice systems** | Not compatible while active |
| **Resource name**       | `pma-voice`                 |
| {.dense}                |                             |

---

## Links

* [Official GitHub Repository](https://github.com/AvarianKnight/pma-voice)

---

## Before You Install

* [ ] Enable OneSync
* [ ] Disable other voice systems
* [ ] Review current convar names
* [ ] Check resources that modify Mumble or network voice natives
* [ ] Test proximity, radio, and call functionality

---

## Credits

Created by **AvarianKnight** and project contributors.

The project credits **Frazzle** and `mumble-voip` for the concept behind the resource.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
