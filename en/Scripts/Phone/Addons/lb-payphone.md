---
title: lb-payphone
description: Paid LB Phone add-on that lets players call people and companies from configured GTA V payphones.
published: true
date: 2026-09-14T01:57:14.726Z
tags: esx, phone, qbcore, script
editor: markdown
dateCreated: 2026-09-14T01:57:14.725Z
---

# lb-payphone [![](https://badges.5metrics.dev/lb-payphone/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-payphone)

Paid LB Phone add-on that lets players call people and companies from configured GTA V payphones.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information            |
| --------------------- | ---------------------- |
| **Name**              | `lb-payphone`          |
| **Creator**           | LB Scripts             |
| **Type**              | Script / Add-on        |
| **Category**          | Phone                  |
| **Game**              | FiveM                  |
| **Price**             | Paid                   |
| **License**           | Unknown                |
| **Framework Support** | QBCore, ESX, custom    |
| **Dependencies**      | `lb-phone`, `loaf_lib` |
| {.dense}              |                        |

---

## Resource Details {.tabset}

### Overview

`lb-payphone` adds usable payphones to LB Phone.

Players can call other players and companies through configured payphone models.

### Requirements

Required:

```text
loaf_lib
lb-phone
```

The authorized store documents support for QBCore, ESX, and standalone/custom integration.

### Interaction

Supported interaction styles include:

* Target interaction
* Press E interaction

The documented target integrations are:

```text
qtarget
qb-target
ox_target
```

---

## Installation

### Installation Checklist

* [ ] Install `loaf_lib`
* [ ] Install `lb-phone`
* [ ] Download `lb-payphone` from the authorized Cfx.re source
* [ ] Place it in your resources folder
* [ ] Configure interaction and calling settings
* [ ] Start it after `lb-phone`
* [ ] Test player and company calls

### Resource Order

```cfg
start loaf_lib
start lb-phone
start lb-payphone
```

---

## Configuration {.tabset}

### Framework

Framework detection is automatic.

It can be set manually through:

```lua
Config.Framework
```

Documented values include:

```text
esx
qb
custom
```

### Interaction

Configure interaction through:

```lua
Config.InteractStyle
```

Available documented styles are:

```text
target
press
```

### Calls

Call pricing is configured through:

```lua
Config.PricePerSecond
```

Unanswered-call timeout is configured through:

```lua
Config.NoAnswerTimeout
```

Company calls can be controlled through the corresponding configuration option.

### Locations

`Config.LocationLocked` can restrict the system to specified payphone coordinates.

Usable payphone models are controlled through:

```lua
Config.Models
```

---

## Links

* [Official Documentation](https://docs.lbscripts.com/payphone/)
* [Installation](https://docs.lbscripts.com/payphone/installation/)
* [Configuration](https://docs.lbscripts.com/payphone/configuration/)
* [Authorized Purchase Page](https://store.lbscripts.com/package/5932915)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
