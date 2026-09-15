---
title: lb-lookupapp
description: Paid LB Phone app for looking up player and vehicle information.
published: true
date: 2026-09-14T01:54:36.159Z
tags: esx, phone-app, qbcore, script
editor: markdown
dateCreated: 2026-09-14T01:54:36.159Z
---

# lb-lookupapp [![](https://badges.5metrics.dev/lb-lookupapp/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-lookupapp)

Paid LB Phone app for looking up player and vehicle information.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information                  |
| --------------------- | ---------------------------- |
| **Name**              | `lb-lookupapp`               |
| **Creator**           | LB Scripts                   |
| **Type**              | Script / Phone App           |
| **Category**          | Lookup                       |
| **Game**              | FiveM                        |
| **Price**             | Paid                         |
| **License**           | FiveM Asset Escrow protected |
| **Framework Support** | QBCore, ESX                  |
| **Dependency**        | `lb-phone`                   |
| {.dense}              |                              |

---

## Resource Details {.tabset}

### Overview

`lb-lookupapp` adds player and vehicle lookup functionality to LB Phone.

The authorized store documents:

* Citizen lookup
* Vehicle lookup
* Configurable visible information
* Hidden persons
* Hidden vehicles
* Locale support

### Requirements

The authorized purchase page lists:

* ESX or QBCore
* `lb-phone`
* `oxmysql`

The product uses FiveM Asset Escrow.

---

## Installation

### Installation Checklist

* [ ] Install `lb-phone`
* [ ] Install `oxmysql`
* [ ] Download `lb-lookupapp` from the authorized source
* [ ] Place it in your resources folder
* [ ] Configure visibility settings
* [ ] Start it after `lb-phone`
* [ ] Test player and vehicle searches

### Resource Order

```cfg
start lb-phone
start lb-lookupapp
```

---

## Configuration

Framework detection is automatic.

If required, configure:

```lua
Config.Framework = "esx"
```

or:

```lua
Config.Framework = "qb"
```

Lookup visibility can be controlled through:

```lua
Config.VisibleInformation
Config.HiddenPersons
Config.HiddenVehicles
```

---

## Links

* [Official Documentation](https://docs.lbscripts.com/lookup/)
* [Installation](https://docs.lbscripts.com/lookup/installation/)
* [Configuration](https://docs.lbscripts.com/lookup/configuration/)
* [Authorized Purchase Page](https://store.lbscripts.com/package/5660717)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
