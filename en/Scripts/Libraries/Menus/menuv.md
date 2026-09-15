---
title: menuv
description: Standalone FiveM NUI menu library for creating buttons, sliders, checkboxes, lists, and other menu interfaces.
published: true
date: 2026-09-14T02:12:51.230Z
tags: library, menus, nui, standalone
editor: markdown
dateCreated: 2026-09-14T02:12:51.230Z
---

# menuv [![](https://badges.5metrics.dev/menuv/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/menuv)

Standalone FiveM NUI menu library for creating buttons, sliders, checkboxes, lists, and other menu interfaces.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information  |
| ------------- | ------------ |
| **Name**      | `menuv`      |
| **Project**   | MenuV        |
| **Creator**   | ThymonA      |
| **Type**      | Library      |
| **Category**  | Menu Library |
| **Game**      | FiveM        |
| **License**   | GPL-3.0      |
| **Framework** | Standalone   |
| {.dense}      |              |

---

## Resource Details {.tabset}

### Overview

MenuV is a FiveM menu library based on NUI.

Documented interface elements include:

* Buttons
* Sliders
* Checkboxes
* Lists
* Confirm controls
* Item descriptions
* Custom RGB colors
* Emojis
* Rebindable keys
* Event-based callbacks

The library includes default and native-style themes.

### Development

MenuV uses Vue.js, TypeScript, and Node.js for its frontend build.

Developers use the library API from their own FiveM resources.

---

## Installation

### Installation Checklist

* [ ] Download `menuv` from the official repository
* [ ] Place `menuv` in your resources folder
* [ ] Start `menuv`
* [ ] Start resources that use MenuV
* [ ] Test menus at the resolutions used by your players

### Resource Order

```cfg
ensure menuv
```

Start dependent resources after the library when they require it during initialization.

---

## Usage

Example API methods documented by the project include:

```lua
menu:AddButton(...)
menu:AddRange(...)
menu:AddCheckbox(...)
menu:AddSlider(...)
```

Menu and item callbacks can be registered with:

```lua
menu:On(...)
item:On(...)
```

Use the project documentation and `example.lua` for current API usage.

---

## Links

* [Official GitHub Repository](https://github.com/ThymonA/menuv)

---

## Credits

Created by **ThymonA** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
