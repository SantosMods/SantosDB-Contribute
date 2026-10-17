---
title: qb-vehicleshop
description: Vehicle dealership for QBCore with test drives, financing, and job-managed private shops.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, qbcore, free, github, vehicles, dealership
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# qb-vehicleshop [![](https://badges.5metrics.dev/qb-vehicleshop/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/qb-vehicleshop)

Vehicle dealership for QBCore with test drives, financing, and job-managed private shops.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information      |
| ------------- | ---------------- |
| **Name**      | `qb-vehicleshop` |
| **Creator**   | QBCore Framework |
| **Type**      | Script           |
| **Category**  | Vehicle Shop     |
| **Game**      | FiveM            |
| **Price**     | Free             |
| **License**   | GPL-3.0          |
| **Framework** | QBCore           |
| **Version**   | `2.1.0`          |
| **Source**    | GitHub           |
| {.dense}      |                  |

---

## Resource Details {.tabset}

### Overview

`qb-vehicleshop` lets players buy vehicles and lets jobs manage shops. The README documents test drives, financing, and free-use or job-managed shops.

### Requirements

* `qb-core`
* `PolyZone`
* `qb-menu`
* `qb-input`
* `oxmysql`

### Features

* Configurable test drive time that returns the player when it ends
* Financing with configurable down payment and maximum payments
* Commission for salespeople at private dealerships
* Shops locked to a job
* Shop areas defined with PolyZone shapes

---

## Installation

### Installation Checklist

* [ ] Install `qb-core`
* [ ] Install `PolyZone`
* [ ] Install `qb-menu`
* [ ] Install `qb-input`
* [ ] Install `oxmysql`
* [ ] Download `qb-vehicleshop` from the official repository
* [ ] Place `qb-vehicleshop` in your resources folder
* [ ] Review `config.lua` where present
* [ ] Start `qb-vehicleshop` after its dependencies
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure qb-core
ensure PolyZone
ensure qb-menu
ensure qb-input
ensure qb-vehicleshop
```

---

## Configuration

Shops are defined in `Config.Shops` with a PolyZone shape. Create new PolyZones if you add a dealership or move the defaults.

Documented options include `Config.Commission`, `Config.FinanceCommission`, `Config.PaymentWarning`, `Config.PaymentInterval`, `Config.MinimumDown`, `Config.MaximumPayments`, and `Config.UsingTarget`.

---

## Links

* [Official Documentation](https://qbcore.org/docs/qbcore-resources/qb-vehicleshop)
* [Official GitHub Repository](https://github.com/qbcore-fivem/qb-vehicleshop)

---

## Credits

Created and maintained by **QBCore Framework** and project contributors.

The repository license credits Joshua Eger.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.