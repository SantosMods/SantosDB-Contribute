---
title: qb-phone
description: QBCore phone resource with garage, mail, banking, racing, MEOS, housing, and downloadable app features.
published: true
date: 2026-09-14T01:29:04.763Z
tags: qbcore, script, ui, phone
editor: markdown
dateCreated: 2026-09-14T01:29:04.763Z
---

# qb-phone [![](https://badges.5metrics.dev/qb-phone/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-phone)

QBCore phone resource with garage, mail, banking, racing, MEOS, housing, and downloadable app features.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information                                                       |
| -------------- | ----------------------------------------------------------------- |
| **Name**       | `qb-phone`                                                        |
| **Creator**    | QBCore Framework                                                  |
| **Type**       | Script                                                            |
| **Category**   | Phone                                                             |
| **Game**       | FiveM                                                             |
| **Price**      | Free                                                              |
| **License**    | GPL-3.0                                                           |
| **Framework**  | QBCore                                                            |
| **Repository** | [qbcore-fivem/qb-phone](https://github.com/qbcore-fivem/qb-phone) |
| {.dense}       |                                                                   |

---

## Resource Details {.tabset}

### Overview

`qb-phone` provides an in-game phone for QBCore.

The official resource includes applications for garages, mail, banking, racing, MEOS, housing, and an app store.

### Requirements

The official repository lists:

* `qb-core`
* `qb-policejob`
* `qb-crypto`
* `qb-lapraces`
* `qb-houses`
* `qb-garages`
* `qb-banking`
* `screenshot-basic`
* A photo-hosting webhook

### Photos

`screenshot-basic` is used for taking photos.

The project also requires a webhook for photo hosting. The repository documents Discord or Imgur as examples.

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Install required application dependencies
* [ ] Install `screenshot-basic`
* [ ] Download `qb-phone`
* [ ] Place it in the `[qb]` directory
* [ ] Import `qb-phone.sql`
* [ ] Configure photo hosting
* [ ] Add resources to your startup configuration
* [ ] Restart the server
* [ ] Test phone applications

### Resource Order

```cfg
ensure qb-core
ensure screenshot-basic
ensure qb-phone
ensure qb-policejob
ensure qb-crypto
ensure qb-lapraces
ensure qb-houses
ensure qb-garages
ensure qb-banking
```

---

## Configuration {.tabset}

### Phone Settings

The repository uses `config.lua` for phone configuration.

Documented settings include:

```lua
Config.RepeatTimeout = 2000
Config.CallRepeats = 10
Config.OpenPhone = 244
```

### Applications

Applications are configured through `Config.PhoneApplications`.

App configuration can control values such as:

* App route
* Icon
* Tooltip
* Job requirement
* Blocked jobs
* App position
* Alert count

### Photo Webhook

Configure the `WebHook` value used by the phone's photo system according to the official repository instructions.

Do not publish private webhook URLs.

---

## Compatibility

| Item                 | Information        |
| -------------------- | ------------------ |
| **Game**             | FiveM              |
| **Framework**        | QBCore             |
| **Database setup**   | Required           |
| **Photo dependency** | `screenshot-basic` |
| **Resource name**    | `qb-phone`         |
| {.dense}             |                    |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-phone)

---

## Before You Install

* [ ] Import `qb-phone.sql`
* [ ] Install the applications your phone configuration uses
* [ ] Configure the photo webhook securely
* [ ] Confirm `screenshot-basic` works
* [ ] Test banking, garages, MEOS, housing, and racing integrations that you enable

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
