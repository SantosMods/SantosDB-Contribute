---
title: lb-phone
description: Paid FiveM phone system with configurable apps, framework integrations, media uploading, and phone functionality.
published: true
date: 2026-09-14T01:51:02.078Z
tags: esx, phone, qbcore, script
editor: markdown
dateCreated: 2026-09-14T01:51:02.078Z
---

# lb-phone [![](https://badges.5metrics.dev/lb-phone/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-phone)

Paid FiveM phone system with configurable apps, framework integrations, media uploading, and phone functionality.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information                               |
| --------------------- | ----------------------------------------- |
| **Name**              | `lb-phone`                                |
| **Creator**           | LB Scripts                                |
| **Type**              | Script                                    |
| **Category**          | Phone                                     |
| **Game**              | FiveM                                     |
| **Price**             | Paid                                      |
| **License**           | Unknown                                   |
| **Framework Support** | QBCore, ESX, custom framework integration |
| {.dense}              |                                           |

---

## Resource Details {.tabset}

### Overview

`lb-phone` is the main LB Scripts phone resource for FiveM.

It includes configurable phone applications and integrations for framework, inventory, vehicles, companies, media uploads, and other server systems.

### Requirements

The official installation documentation requires:

* `oxmysql`
* Up-to-date FiveM server artifacts
* MariaDB 10.11 or newer

`loaf_bcrypt` is recommended.

OneSync Infinity is optional but required for features such as AirShare.

### Framework Support

The documentation provides built-in QBCore and ESX integration files.

Custom frameworks can be implemented using the supplied standalone framework files.

---

## Installation

> Back up your database before making database changes.
> {.is-danger}

### Installation Checklist

* [ ] Install MariaDB 10.11 or newer
* [ ] Install `oxmysql`
* [ ] Install `loaf_bcrypt` if desired
* [ ] Download `lb-phone` from the authorized source
* [ ] Remove old `phone_` tables when performing the documented fresh installation
* [ ] Import `lb-phone/phone.sql` using HeidiSQL
* [ ] Configure upload API keys
* [ ] Start dependencies before `lb-phone`
* [ ] Restart the server
* [ ] Test calls, apps, media uploads, and framework integration

### Resource Order

```cfg
start oxmysql
start lb-phone
```

When using `loaf_bcrypt`:

```cfg
add_unsafe_worker_permission loaf_bcrypt
start loaf_bcrypt
start lb-phone
```

> Custom LB Phone apps should start after `lb-phone`.
> {.is-info}

---

## Configuration

The phone configuration is stored in the resource's `config` folder.

Upload API keys are configured in:

```text
lb-phone/server/apiKeys.lua
```

The phone automatically detects supported frameworks by default.

Custom framework integrations can use:

```text
lb-phone/client/custom/frameworks/standalone.lua
lb-phone/server/custom/frameworks/standalone.lua
```

---

## Known Issues

The official documentation warns against using XAMPP and phpMyAdmin for the documented database installation.

Database errors can occur when MariaDB is outdated or phone database updates have not been applied.

OneSync Infinity is required for AirShare functionality.

---

## Links

* [Official Documentation](https://docs.lbscripts.com/phone/)
* [Installation](https://docs.lbscripts.com/phone/installation/)
* [Configuration](https://docs.lbscripts.com/phone/configuration/)
* [Authorized Store](https://store.lbscripts.com/)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
