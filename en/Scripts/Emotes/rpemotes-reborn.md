---
title: rpemotes-reborn
description: Community-driven FiveM emote menu with animations, facial expressions, walk styles, props, shared emotes, and framework support.
published: true
date: 2026-09-14T23:57:14.523Z
tags: esx, qbcore, script, emotes
editor: markdown
dateCreated: 2026-09-14T23:57:14.523Z
---

# rpemotes-reborn [![](https://badges.5metrics.dev/rpemotes-reborn/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/rpemotes-reborn)

Community-driven FiveM emote menu with animations, facial expressions, walk styles, props, shared emotes, and framework support.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field                    | Information                          |
| ------------------------ | ------------------------------------ |
| **Name**                 | `rpemotes-reborn`                    |
| **Creator / Maintainer** | alberttheprince / RPEmotes community |
| **Type**                 | Script                               |
| **Category**             | Emotes                               |
| **Game**                 | FiveM                                |
| **Price**                | Free                                 |
| **License**              | GPL-3.0                              |
| **Framework Support**    | QBCore, ESX                          |
| {.dense}                 |                                      |

## Resource Details {.tabset}

### Overview

`rpemotes-reborn` is a community-driven FiveM emote menu.

Documented functionality includes:

* Emote preview and placement
* Emote search
* Custom animations
* Group emotes
* Exit emotes
* Facial expressions
* Walk styles
* Props
* Animal emotes
* Shared particle effects
* Shared and couple animations
* Crouching
* Crawling
* Finger pointing
* Ragdoll
* Hands up
* Binoculars
* News camera
* Custom categories

### Framework Support

The project documents QBCore and ESX support.

For QBCore, configure:

```lua
Framework = 'qb-core'
```

### Exports

Current exports include:

```lua
exports["rpemotes-reborn"]:Execute(emoteName, emoteType, textureVariation)
exports["rpemotes-reborn"]:EmoteCancel(forceCancel)
exports["rpemotes-reborn"]:IsPlayerCrouched()
exports["rpemotes-reborn"]:IsPlayerProne()
exports["rpemotes-reborn"]:IsPlayerCrawling()
exports["rpemotes-reborn"]:IsPlayerPointing()
exports["rpemotes-reborn"]:IsPlayerInAnim()
exports["rpemotes-reborn"]:IsPlayerInHandsUp()
exports["rpemotes-reborn"]:toggleBinoculars()
```

`EmoteCommandStart` remains documented but is deprecated in favor of `Execute()`.

## Installation

### Installation Checklist

* [ ] Download an official release
* [ ] Use current recommended FiveM artifacts
* [ ] Configure `config.lua`
* [ ] Select the required framework
* [ ] Configure `MenuLanguage`
* [ ] Enable OneSync Infinity when using particle effects
* [ ] Enforce an appropriate current game build for supported emotes and props
* [ ] Start the resource
* [ ] Test custom and shared emotes

> The repository is named `rpemotes-reborn`, but the official installation instructions use `rpemotes` as the installed resource folder/start name.
> {.is-info}

```cfg
ensure rpemotes
```

### Updating Custom Animations

> `AnimationListCustom.lua` and `BackUpAnimationListCustom.lua` from versions before 1.5.0 are not compatible with version 1.5.0 and later in the manner documented by the project.
> {.is-warning}

Copy your custom animation entries into the current release files instead of replacing them with incompatible older files.

Keep a backup of your configuration and custom animations before upgrading.

## Compatibility

| Item                        | Information                                       |
| --------------------------- | ------------------------------------------------- |
| **Game**                    | FiveM                                             |
| **QBCore**                  | Supported                                         |
| **ESX**                     | Supported                                         |
| **OneSync Infinity**        | Required for particle effects to work as intended |
| **Installed resource name** | `rpemotes`                                        |
| {.dense}                    |                                                   |

## Links

* [Official GitHub Repository](https://github.com/alberttheprince/rpemotes-reborn)
* [Official Releases](https://github.com/alberttheprince/rpemotes-reborn/releases)
* [Official Documentation](https://rpemotes-reborn.gitbook.io/guide)

## Credits

Maintained by **alberttheprince** and the **RPEmotes community**.

The project credits its community contributors and the creators who permitted their custom animations and props to be included. The project specifically states that contributed custom animation and prop content was added with creator permission and is intended to remain free.

SantosDB provides resource information and source references.

Resource rights belong to the project authors, animation creators, contributors, and other applicable rights holders.
