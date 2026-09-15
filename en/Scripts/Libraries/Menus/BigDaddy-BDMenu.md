---
title: BigDaddy-BDMenu
description: Free developer menu resource that opens JSON-defined or dynamically generated menus while retaining keyboard and mouse game control.
published: true
date: 2026-09-13T17:56:57.584Z
tags: developer-tool, library, menus, standalone
editor: markdown
dateCreated: 2026-09-13T17:56:57.584Z
---

# BDMenu [![](https://badges.5metrics.dev/BigDaddy-BDMenu/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-BDMenu)

BDMenu is a free menu resource for creating in-game menus from JSON or client-side events.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `BDMenu`                 |
| **Resource Folder** | `BigDaddy-BDMenu`        |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Library / Developer Tool |
| **Category**        | Menus                    |
| **Version**         | `v1.0.0`                 |
| **Price**           | Free                     |
| **Dependencies**    | None                     |
| **QBCore / Qbox**   | ✔ Stand-Alone compatible |
| **ESX**             | ✔ Stand-Alone compatible |
| {.dense}            |                          |

BDMenu lets the player retain mouse and keyboard control while the menu is open. The menu itself can be controlled with arrow keys, Enter, and Backspace.

---

## Resource Details {.tabset}

### Overview

BDMenu is intended for developers who need a reusable FiveM menu.

Menus can be created from JSON data or constructed dynamically and passed to BDMenu from another client resource.

### Features

* JSON-based menu definitions
* Dynamically generated menus
* Nested submenus
* Commands
* Client events
* Server events
* Optional event payloads
* Disabled menu items
* Permission-controlled items
* Optional icons
* Font Awesome icon support
* Image icon support
* Keep normal game controls available while the menu is open

---

## Installation

### Installation Checklist

* [ ] Download BDMenu from Big Daddy Scripts.
* [ ] Place `BigDaddy-BDMenu` in your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-BDMenu
```

> Do not rename `BigDaddy-BDMenu`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration

The `settings.ini` file contains the product key.

| Setting  | Default | Description                   |
| -------- | ------- | ----------------------------- |
| `key1`   | `none`  | Big Daddy Scripts product key |
| {.dense} |         |                               |

---

## Client Events

Open a menu:

```lua
TriggerEvent('BigDaddy-BDMenu:OpenMenu', json.encode(menu))
```

Close the current menu:

```lua
TriggerEvent('BigDaddy-BDMenu:CloseMenu')
```

---

## Menu Format

BDMenu accepts either:

* A raw array of items
* An object containing `title` and `items`

Supported item fields include:

| Field                                         | Purpose                                          |
| --------------------------------------------- | ------------------------------------------------ |
| `description`, `name`, `label`, `title`, `id` | Menu item text                                   |
| `items`                                       | Nested submenu                                   |
| `actionType`                                  | Defines command or event behavior                |
| `action`                                      | Command or event name                            |
| `payload`                                     | Optional command or event data                   |
| `close`                                       | Controls whether the menu closes after selection |
| `disabled` / `Disabled`                       | Disables the option                              |
| `icon`                                        | Icon name or Font Awesome class                  |
| `iconUrl` / `iconPath`                        | Explicit image source                            |
| `permission`                                  | Permission key                                   |
| `permissionMode`                              | `disable` or `hide`                              |
| `hideIfNoPermission`                          | Boolean alias for hide behavior                  |
| {.dense}                                      |                                                  |

Supported actions include:

```text
command
event
clientEvent
client
serverEvent
server
netEvent
```

---

## Permissions

Menu items without a `permission` value are unrestricted.

If a permission is present and denied:

* Default behavior disables the item.
* `permissionMode: "hide"` removes the item.
* `hideIfNoPermission: true` also removes the item.

Permission evaluation relies on the permission data supplied to the menu implementation.

---

## Icons

BDMenu supports common image formats:

```text
PNG
JPG
JPEG
WEBP
GIF
SVG
```

Font Awesome icon classes are also supported.

For icons stored in another resource, the documentation supports FiveM NUI URLs such as:

```text
nui://my-resource/html/icons/cop.svg
```

---

## Compatibility

| Platform        | Status                               |
| --------------- | ------------------------------------ |
| **Stand-Alone** | Supported                            |
| **QBCore**      | ✔ Verified Stand-Alone compatibility |
| **Qbox**        | ✔ Verified Stand-Alone compatibility |
| **ESX**         | ✔ Verified Stand-Alone compatibility |
| {.dense}        |                                      |

---

## Official Links

* [BDMenu Product Page](https://bigdaddyscripts.com/Products/View/3392/BDMenu)
* [BDMenu Documentation](https://wiki.bigdaddyscripts.com/Documentation/BDMenu/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
