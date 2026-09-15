---
title: lb-newsapp
description: Paid LB Phone news app for publishing and reading articles with categories, profiles, permissions, and search.
published: true
date: 2026-09-14T01:55:12.488Z
tags: esx, qbcore, script, news
editor: markdown
dateCreated: 2026-09-14T01:55:12.488Z
---

# lb-newsapp [![](https://badges.5metrics.dev/lb-newsapp/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-newsapp)

Paid LB Phone news app for publishing and reading articles with categories, profiles, permissions, and search.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information                             |
| --------------------- | --------------------------------------- |
| **Name**              | `lb-newsapp`                            |
| **Creator**           | LB Scripts                              |
| **Type**              | Script / Phone App                      |
| **Category**          | News                                    |
| **Game**              | FiveM                                   |
| **Price**             | Paid                                    |
| **License**           | FiveM Asset Escrow protected            |
| **Framework Support** | QBCore, ESX, custom framework templates |
| **Dependency**        | `lb-phone`                              |
| {.dense}              |                                         |

---

## Resource Details {.tabset}

### Overview

`lb-newsapp` adds a news application to LB Phone.

It lets authorized reporters create articles while players can browse and search published content.

Documented functionality includes:

* Articles
* Categories
* Reporter profiles
* Search
* Configurable permissions
* Action logs
* Discord publication notifications

### Requirements

Required:

```text
lb-phone
```

The authorized store states that the resource is preconfigured for ESX and QBCore and includes template files for implementing another framework.

The product uses FiveM Asset Escrow.

---

## Installation

### Installation Checklist

* [ ] Install `lb-phone`
* [ ] Download `lb-newsapp` from the authorized source
* [ ] Place it in your resources folder
* [ ] Import `news.sql`
* [ ] Configure the reporter job
* [ ] Start it after `lb-phone`
* [ ] Test article creation and viewing

### Resource Order

```cfg
start lb-phone
start lb-newsapp
```

### Database

Import:

```text
news.sql
```

using HeidiSQL.

For ESX, the package includes:

```text
esx.sql
```

to add the `reporter` job.

QBCore servers must add the `reporter` job to their QBCore job configuration.

---

## Configuration

The resource automatically detects the framework.

Common settings include:

```lua
Config.Framework
Config.Language
Config.JobName
Config.Permissions
```

Logging supports services documented by LB Scripts, including `fivemanage`, `ox_lib`, and Discord.

---

## Links

* [Official Documentation](https://docs.lbscripts.com/news-app/)
* [Installation](https://docs.lbscripts.com/news-app/installation/)
* [Configuration](https://docs.lbscripts.com/news-app/configuration/)
* [Authorized Purchase Page](https://store.lbscripts.com/package/6399882)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
