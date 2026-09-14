---
title: qb-banking
description: QBCore banking system for player, job, gang, and shared accounts with bank and ATM interactions.
published: true
date: 2026-09-14T01:31:42.862Z
tags: banking, qbcore, script, shared-accounts
editor: markdown
dateCreated: 2026-09-14T01:31:42.862Z
---

# qb-banking [![](https://badges.5metrics.dev/qb-banking/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-banking)

QBCore banking system for player, job, gang, and shared accounts with bank and ATM interactions.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-banking`     |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Banking          |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-banking` handles banking for player, job, gang, and shared accounts.

Documented features include:

* Bank and ATM interactions
* Bank card integration
* Shared player accounts
* Automatic job and gang account creation when first opened
* Boss-only access to job and gang accounts

### Database

The repository includes `banking.sql`.

Import the current SQL file when required by your installation.

### Exports

The official documentation provides server exports for managing accounts and transactions.

Use the current QBCore documentation for export names and parameters.

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Download `qb-banking`
* [ ] Place `qb-banking` in your `[qb]` resources
* [ ] Import `banking.sql`
* [ ] Review `config.lua`
* [ ] Add the resource to your startup configuration
* [ ] Restart the server
* [ ] Test player and shared accounts

### Resource Order

```cfg
ensure qb-core
ensure qb-banking
```

---

## Configuration

Review `config.lua` before starting the resource.

Test bank locations, ATM interactions, account access, and any integrations used by your server.

---

## Compatibility

| Item              | Information   |
| ----------------- | ------------- |
| **Game**          | FiveM         |
| **Framework**     | QBCore        |
| **Database file** | `banking.sql` |
| **Resource name** | `qb-banking`  |
| {.dense}          |               |

---

## Links

* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-banking)
* [Official QBCore Documentation](https://docs.qbcore.org/qbcore-documentation/qbcore-resources/qb-banking)

---

## Before You Install

* [ ] Back up your database
* [ ] Import the current database schema
* [ ] Review account configuration
* [ ] Test job and gang account permissions
* [ ] Test shared accounts and ATM access

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
