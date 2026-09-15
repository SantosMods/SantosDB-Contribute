---
title: ox_banking
description: Banking system for ox_core with personal, shared, and group accounts, invoices, transaction logs, and ATMs.
published: true
date: 2026-09-14T02:16:04.699Z
tags: banking, script, shared-accounts, ox-core
editor: markdown
dateCreated: 2026-09-14T02:16:04.699Z
---

# ox_banking [![](https://badges.5metrics.dev/ox_banking/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/ox_banking)

Banking system for `ox_core` with personal, shared, and group accounts, invoices, transaction logs, and ATMs.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information  |
| ------------- | ------------ |
| **Name**      | `ox_banking` |
| **Creator**   | Overextended |
| **Type**      | Script       |
| **Category**  | Banking      |
| **Game**      | FiveM        |
| **License**   | MIT          |
| **Framework** | `ox_core`    |
| {.dense}      |              |

---

## Resource Details {.tabset}

### Overview

`ox_banking` is a banking system built specifically for `ox_core`.

Documented banking functionality includes:

* Personal accounts
* New account creation
* Shared accounts
* Group accounts
* Deposits
* Withdrawals
* Transfers
* Invoices
* Account transaction logs
* Shared-account access management
* Group-grade access
* ATMs

### Requirements

Required dependencies:

* `ox_core`
* `ox_inventory`
* `ox_lib`
* `oxmysql`

### Accounts

Personal accounts can be converted to shared accounts.

Shared accounts include access management.

Group accounts can restrict access according to group grades.

---

## Installation

### Installation Checklist

* [ ] Install `ox_core`
* [ ] Install `ox_inventory`
* [ ] Install `ox_lib`
* [ ] Install `oxmysql`
* [ ] Download the latest official `ox_banking` release
* [ ] Configure the resource
* [ ] Start dependencies before `ox_banking`
* [ ] Test accounts, invoices, and ATMs

### Resource Order

```cfg
ensure oxmysql
ensure ox_lib
ensure ox_core
ensure ox_inventory
ensure ox_banking
```

Check the current dependency documentation for the complete startup order used by your Overextended stack.

---

## Compatibility

| Item              | Information    |
| ----------------- | -------------- |
| **Game**          | FiveM          |
| **Framework**     | `ox_core`      |
| **Inventory**     | `ox_inventory` |
| **Library**       | `ox_lib`       |
| **Database**      | `oxmysql`      |
| **Resource name** | `ox_banking`   |
| {.dense}          |                |

---

## Links

* [Official GitHub Repository](https://github.com/overextended/ox_banking)
* [Official Releases](https://github.com/overextended/ox_banking/releases)

---

## Credits

Created and maintained by **Overextended** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
