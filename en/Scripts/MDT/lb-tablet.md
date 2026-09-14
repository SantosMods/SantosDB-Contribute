---
title: lb-tablet
description: Paid FiveM tablet system with configurable MDT functionality, custom apps, and script integration exports.
published: true
date: 2026-09-14T01:52:22.924Z
tags: mdt, script, ui, tablet
editor: markdown
dateCreated: 2026-09-14T01:52:22.924Z
---

# lb-tablet [![](https://badges.5metrics.dev/lb-tablet/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-tablet)

Paid FiveM tablet system with configurable MDT functionality, custom apps, and script integration exports.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field        | Information  |
| ------------ | ------------ |
| **Name**     | `lb-tablet`  |
| **Creator**  | LB Scripts   |
| **Type**     | Script       |
| **Category** | Tablet / MDT |
| **Game**     | FiveM        |
| **Price**    | Paid         |
| **License**  | Unknown      |
| {.dense}     |              |

---

## Resource Details {.tabset}

### Overview

`lb-tablet` provides a configurable FiveM tablet with MDT functionality for police and EMS.

It supports custom apps and exports for integration with other server scripts.

### Requirements

The official installation documentation requires:

* `oxmysql`
* MariaDB 10.11 or newer
* Up-to-date FiveM server artifacts

OneSync Infinity is optional but required for some features such as AirShare.

### Database

The resource can automatically check and repair its database structure when:

```lua
Config.DatabaseChecker.Enabled = true
Config.DatabaseChecker.AutoFix = true
```

If automatic setup is disabled or fails, import:

```text
lb-tablet/tablet.sql
```

using HeidiSQL.

---

## Installation

> Back up your database before changing the tablet database structure.
> {.is-danger}

### Installation Checklist

* [ ] Install MariaDB 10.11 or newer
* [ ] Install `oxmysql`
* [ ] Download `lb-tablet` from the authorized source
* [ ] Configure the database checker or import `tablet.sql`
* [ ] Add the `tablet` item if item access is required
* [ ] Configure upload API keys
* [ ] Start dependencies before `lb-tablet`
* [ ] Test MDT and custom app integrations

### Resource Order

```cfg
start oxmysql
start lb-tablet
```

---

## Configuration

The main configuration is located at:

```text
lb-tablet/config/config.lua
```

MDTs are configured in:

```text
lb-tablet/config/mdts.json
```

Upload API keys are stored in:

```text
lb-tablet/server/apiKeys.lua
```

Custom framework and inventory integrations can use the supplied standalone files under the client and server `custom/frameworks/standalone/` directories.

---

## Links

* [Official Documentation](https://docs.lbscripts.com/tablet/)
* [Installation](https://docs.lbscripts.com/tablet/installation/)
* [Configuration](https://docs.lbscripts.com/tablet/configuration/)
* [Authorized Store](https://store.lbscripts.com/)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
