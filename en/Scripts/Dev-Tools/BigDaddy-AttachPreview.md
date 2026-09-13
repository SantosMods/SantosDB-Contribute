---
title: BigDaddy-AttachPreview
description: In-game developer tool for visually positioning up to two props on a ped, previewing animations, and generating C#, Lua, or JSON attachment data.
published: true
date: 2026-09-13T17:55:47.270Z
tags: developer-tool, standalone, tool, prop-attachment
editor: markdown
dateCreated: 2026-09-13T17:55:47.270Z
---

# Attach Preview [![](https://badges.5metrics.dev/BigDaddy-AttachPreview/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-AttachPreview)

Attach Preview is an in-game developer tool for positioning props on a player and generating attachment data.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `Attach Preview`         |
| **Resource Folder** | `BigDaddy-AttachPreview` |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Developer Tool           |
| **Category**        | Development              |
| **Version**         | `v1.0.0`                 |
| **Price**           | $3.00 USD                |
| **Dependencies**    | None                     |
| **QBCore / Qbox**   | ✔ Stand-Alone compatible |
| **ESX**             | ✔ Stand-Alone compatible |
| **ACE Permissions** | Supported                |
| {.dense}            |                          |

---

## Resource Details {.tabset}

### Overview

Attach Preview lets developers visually place one or two props on a ped while previewing animations.

Position and rotation changes appear immediately. The tool can then generate C#, Lua, or JSON output containing the current attachment values.

### Features

* Preview one or two props
* Select ped bones
* Adjust position offsets
* Adjust rotation offsets
* Configure rotation order
* Preview animations
* Use preset or custom animations
* Orbit the preview camera
* Generate C# output
* Generate Lua output
* Generate JSON output
* Copy output to clipboard
* ACE permission support

---

## Installation

### Installation Checklist

* [ ] Download Attach Preview from Big Daddy Scripts.
* [ ] Place `BigDaddy-AttachPreview` in your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Configure ACE permissions if required.
* [ ] Configure `settings.json` presets if required.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-AttachPreview
```

> Do not rename `BigDaddy-AttachPreview`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration {.tabset}

### settings.ini

| Setting             | Default          | Description                                               |
| ------------------- | ---------------- | --------------------------------------------------------- |
| `key1`              | `productkeyhere` | Big Daddy Scripts product key                             |
| `UseAcePermissions` | `true`           | Requires the configured ACE permission                    |
| `AcePermission`     | `command`        | ACE permission checked by the resource                    |
| `debug`             | `false`          | Enables additional debugging output                       |
| `DesyncKey`         | various          | Internal synchronization value that should not be changed |
| {.dense}            |                  |                                                           |

Example ACE permission:

```cfg
add_ace group.admin command allow
```

The ACE permission must be configured separately in your server permissions.

### settings.json

| Setting             | Default         | Description                            |
| ------------------- | --------------- | -------------------------------------- |
| `command`           | `attachpreview` | Command used to open the tool          |
| `defaultMoveStep`   | `0.01`          | Default movement adjustment in meters  |
| `defaultRotateStep` | `1.0`           | Default rotation adjustment in degrees |
| `props`             | see file        | Preset prop model list                 |
| `animations`        | see file        | Animation presets                      |
| `bones`             | see file        | Named ped bone IDs                     |
| {.dense}            |                 |                                        |

You can add or remove prop, animation, and bone presets without rebuilding the resource.

Restart `BigDaddy-AttachPreview` after changing `settings.json`.

---

## Usage

Open the tool with:

```text
/attachpreview
```

Your player is frozen while the preview interface is open.

### Prop Preview

For each preview prop:

1. Select a preset or enter a custom model.
2. Select the ped bone.
3. Select the rotation order.
4. Spawn the prop.
5. Adjust X, Y, and Z position.
6. Adjust X, Y, and Z rotation.
7. Use the camera angle control to inspect placement.

### Animation Preview

Select a preset animation or enter:

* Animation dictionary
* Animation name
* Animation flags

You can play and stop the animation while adjusting attached props.

### Generated Output

The Output tab can generate:

```text
C#
Lua
JSON
```

Generated attachment data includes the current:

* Model
* Bone ID
* Position
* Rotation
* Rotation order

> Preview props are temporary and are removed when the tool closes or the resource stops. Copy the generated values before closing the interface.
> {.is-warning}

---

## Compatibility

| Platform            | Status                               |
| ------------------- | ------------------------------------ |
| **Stand-Alone**     | Supported                            |
| **QBCore**          | ✔ Verified Stand-Alone compatibility |
| **Qbox**            | ✔ Verified Stand-Alone compatibility |
| **ESX**             | ✔ Verified Stand-Alone compatibility |
| **ACE Permissions** | Supported                            |
| {.dense}            |                                      |

---

## Official Links

* [Attach Preview Product Page](https://bigdaddyscripts.com/Products/View/3444/Attach-Preview)
* [Attach Preview Documentation](https://wiki.bigdaddyscripts.com/Documentation/Attach-Preview/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
