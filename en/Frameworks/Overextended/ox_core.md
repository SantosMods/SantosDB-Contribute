---
title: ox_core
description: A modern FiveM framework providing player and vehicle management and persistence.
published: true
date: 2026-10-16T12:00:00.000Z
tags: framework, ox-core, free, github, overextended, core
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# ox_core [![](https://badges.5metrics.dev/ox_core/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/ox_core)

A modern FiveM framework providing player and vehicle management and persistence.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

> The repository `LICENSE` file and `package.json` state LGPL-3.0, while `NOTICE.md` states GPL-3.0 or later. Review the official repository before redistributing or publishing modified code.
> {.is-warning}

---

## Resource Information

| Field         | Information       |
| ------------- | ----------------- |
| **Name**      | `ox_core`         |
| **Creator**   | Overextended      |
| **Type**      | Framework         |
| **Category**  | Core Framework    |
| **Game**      | FiveM             |
| **Price**     | Free              |
| **License**   | LGPL-3.0-or-later |
| **Framework** | Ox Core           |
| **Version**   | `1.5.14`          |
| **Source**    | GitHub            |
| {.dense}      |                   |

---

## Resource Details {.tabset}

### Overview

`ox_core` is the Overextended framework for FiveM. The repository describes it as player and vehicle management and persistence.

Third-party resources built for the framework should not use the `ox` prefix, according to the project README.

### Requirements

* `oxmysql`
* `ox_lib`
* MariaDB 11.4 or newer (per the official documentation)

### Features

* Lua definitions through `@ox_core/lib/init.lua`
* JavaScript and TypeScript support through the `@overextended/ox_core` npm package
* Configuration through convars
* Optional integrations: `ox_inventory`, `npwd`, `illenium-appearance`

---

## Installation

### Installation Checklist

* [ ] Install MariaDB 11.4 or newer
* [ ] Install `oxmysql` and `ox_lib`
* [ ] Download the latest `ox_core` release, or build from source
* [ ] Place `ox_core` in your resources folder
* [ ] Configure the `ox_core` convars
* [ ] Start `ox_core` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure oxmysql
ensure ox_lib
ensure ox_core
```

> Building from source needs Git, Node.js, and bun. The official documentation also offers a txAdmin recipe for a quick setup.
> {.is-info}

---

## Using ox_core in Your Resources

Lua:

```lua
shared_script '@ox_core/lib/init.lua'
```

JavaScript:

```bash
bun i @overextended/ox_core
```

---

## Links

* [Official Documentation](https://overextended.dev/docs/ox_core)
* [GitHub Repository](https://github.com/overextended/ox_core)
* [Latest Release](https://github.com/overextended/ox_core/releases/latest)
* [txAdmin Recipe](https://github.com/overextended/txAdminRecipe)
* [npm Package](https://www.npmjs.com/package/@overextended/ox_core)
* [Cfx.re Release Thread](https://forum.cfx.re/t/ox-core-a-modern-fivem-framework/5276507)
* [Overextended](https://overextended.dev/)

---

## Credits

Created by **Overextended** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.