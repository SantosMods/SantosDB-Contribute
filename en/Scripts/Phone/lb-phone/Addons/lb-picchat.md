---
title: lb-picchat
description: Paid LB Phone application installed as lb-picchat with its own SQL data and configurable locales.
published: true
date: 2026-09-14T01:56:32.110Z
tags: phone-app, script, social, media
editor: markdown
dateCreated: 2026-09-14T01:56:32.110Z
---

# lb-picchat [![](https://badges.5metrics.dev/lb-picchat/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-picchat)

Paid LB Phone application installed as `lb-picchat` with its own SQL data and configurable locales.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field          | Information        |
| -------------- | ------------------ |
| **Name**       | `lb-picchat`       |
| **Creator**    | LB Scripts         |
| **Type**       | Script / Phone App |
| **Category**   | Social App         |
| **Game**       | FiveM              |
| **Price**      | Paid               |
| **License**    | Unknown            |
| **Dependency** | `lb-phone`         |
| {.dense}       |                    |

---

## Requirements

Required:

```text
lb-phone
```

---

## Installation

> Back up your database before importing or changing SQL data.
> {.is-danger}

### Installation Checklist

* [ ] Install `lb-phone`
* [ ] Download `lb-picchat` from the authorized Cfx.re source
* [ ] Place it in your resources folder
* [ ] Import `picchat.sql` using HeidiSQL
* [ ] Configure the resource
* [ ] Start it after `lb-phone`
* [ ] Test the app in LB Phone

### Resource Order

```cfg
start lb-phone
start lb-picchat
```

### Database

Import:

```text
picchat.sql
```

using HeidiSQL.

---

## Configuration

The language is controlled through:

```lua
Config.Language
```

Locale files are stored under:

```text
lb-picchat/config/locales
```

---

## Links

* [Official Installation Documentation](https://docs.lbscripts.com/picchat/installation/)
* [Official Configuration Documentation](https://docs.lbscripts.com/picchat/configuration/)
* [Authorized Store](https://store.lbscripts.com/)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
