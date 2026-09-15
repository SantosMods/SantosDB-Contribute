---
title: MenuAPI
description: C# menu API for FiveM and RedM designed as a NativeUI replacement and used by resources such as vMenu.
published: true
date: 2026-09-14T02:13:59.601Z
tags: developer-tool, library, menus, standalone
editor: markdown
dateCreated: 2026-09-14T02:13:59.601Z
---

# MenuAPI [![](https://badges.5metrics.dev/MenuAPI/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/MenuAPI)

C# menu API for FiveM and RedM designed as a NativeUI replacement.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field        | Information    |
| ------------ | -------------- |
| **Name**     | `MenuAPI`      |
| **Creator**  | Tom Grobbe     |
| **Type**     | Library        |
| **Category** | Menu API       |
| **Games**    | FiveM, RedM    |
| **Price**    | Free           |
| **License**  | Custom license |
| **Language** | C#             |
| {.dense}     |                |

---

## Resource Details {.tabset}

### Overview

MenuAPI is a C# menu library designed as a replacement for NativeUI.

It supports FiveM and RedM and includes safezone alignment support for FiveM.

### Installation Model

MenuAPI is intended for resource developers.

The official repository provides two integration methods:

* Reference the appropriate release `MenuAPI.dll`
* Install the relevant NuGet package

MenuAPI is normally included as a dependency inside the developer's resource rather than installed as a standalone server resource.

### License

MenuAPI uses a custom license.

The license allows its pre-built files to be included in commercial and non-commercial projects, but imposes restrictions on selling or redistributing MenuAPI itself.

Review the official license before redistributing or modifying the library.

---

## Developer Installation

Add the library reference to your C# project and import:

```csharp
using MenuAPI;
```

When publishing the resource, include:

```lua
files {
    'MenuAPI.dll'
}
```

Keep `MenuAPI.dll` in the resource folder.

---

## Compatibility

| Item                               | Information  |
| ---------------------------------- | ------------ |
| **FiveM**                          | Supported    |
| **RedM**                           | Supported    |
| **Language**                       | C#           |
| **Standalone server installation** | Not intended |
| {.dense}                           |              |

---

## Links

* [Official GitHub Repository](https://github.com/TomGrobbe/MenuAPI)
* [Official Documentation](https://docs.vespura.com/mapi/)

---

## Credits

Created by **Tom Grobbe** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
