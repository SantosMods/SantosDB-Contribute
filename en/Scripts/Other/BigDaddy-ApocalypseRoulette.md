---
title: BigDaddy-ApocalypseRoulette
description: Lets players wager configured ox_inventory items on a roulette wheel for multiplied rewards, losses, or a lethal skull result.
published: true
date: 2026-09-13T18:03:24.223Z
tags: inventory-game, qbcore, qbox, script
editor: markdown
dateCreated: 2026-09-13T17:54:07.756Z
---

# Apocalypse Roulette [![](https://badges.5metrics.dev/BigDaddy-ApocalypseRoulette/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-ApocalypseRoulette)

Apocalypse Roulette lets players wager inventory items on a configurable roulette wheel.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information                   |
| ------------------- | ----------------------------- |
| **Name**            | `Apocalypse Roulette`         |
| **Resource Folder** | `BigDaddy-ApocalypseRoulette` |
| **Creator**         | Big Daddy Scripts             |
| **Game**            | FiveM                         |
| **Type**            | Script                        |
| **Category**        | Minigame                      |
| **Version**         | `v1.0.1`                      |
| **Price**           | $10.00 USD                    |
| **Frameworks**      | QBCore, Qbox                  |
| **Inventory**       | `ox_inventory`                |
| **Library**         | `ox_lib`                      |
| **Targeting**       | `ox_target`                   |
| **ESX**             | 🚫 Not implemented            |
| {.dense}            |                               |

The official compatibility table marks QBCore and Qbox with **✅**, meaning framework integration is implemented and verified. ESX is marked **🚫**.

---

## Resource Details {.tabset}

### Overview

Apocalypse Roulette is an apocalypse-themed betting wheel.

Players wager configured inventory items. The result can multiply the wager, lose the wager, or trigger the skull result, which kills the player.

### Features

* Inventory-item wagering
* Configurable allowed items
* Configurable minimum and maximum wagers
* Configurable cooldown
* Multiple wheel locations
* Configurable wheel timing
* `ox_inventory` integration
* `ox_target` interaction
* QBCore and Qbox support

---

## Requirements

Install these required resources before Apocalypse Roulette:

```text
ox_inventory
ox_lib
ox_target
```

A supported framework is also required:

* QBCore
* Qbox

ESX is not supported by the current official compatibility table.

---

## Installation

### Installation Checklist

* [ ] Install `ox_lib`.
* [ ] Install `ox_inventory`.
* [ ] Install `ox_target`.
* [ ] Confirm QBCore or Qbox is running.
* [ ] Place `BigDaddy-ApocalypseRoulette` in your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Configure `config.json`.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-ApocalypseRoulette
```

> Do not rename `BigDaddy-ApocalypseRoulette`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration {.tabset}

### settings.ini

| Setting                  | Default | Description                                                                    |
| ------------------------ | ------- | ------------------------------------------------------------------------------ |
| `key1`                   | `none`  | Big Daddy Scripts product key                                                  |
| `ShowDisabledBetChoices` | `false` | Shows all allowed items as disabled choices when the player does not have them |
| {.dense}                 |         |                                                                                |

When `ShowDisabledBetChoices=false`, the betting menu only displays eligible items the player currently has.

### config.json

`config.json` controls the roulette wheel configuration.

Documented settings include:

| Setting           |      Default | Description                                         |
| ----------------- | -----------: | --------------------------------------------------- |
| `cooldownSeconds` |       `7200` | Cooldown before the same player can spin again      |
| `syncDistance`    |       `50.0` | Distance at which nearby players see the wheel spin |
| `spinMinMs`       |      `12000` | Minimum wheel spin duration                         |
| `spinMaxMs`       |      `18000` | Maximum wheel spin duration                         |
| `allowedItems`    | configurable | Inventory items that can be wagered                 |
| `wheels`          | configurable | Wheel locations and placement data                  |
| {.dense}          |              |                                                     |

Each allowed item can define:

* Inventory item name
* Display label
* Minimum wager
* Maximum wager

Multiple roulette wheels can be configured.

---

## Usage

Walk to a configured wheel and use the third-eye interaction to select **SPIN WHEEL**.

The script opens the bet menu. Select an eligible inventory item and quantity.

The wheel result determines the outcome:

* Number result: wager multiplied by the landed number
* Loser result: wager is lost
* Skull result: player explodes

The configured cooldown begins after the spin.

---

## Compatibility

| Platform / Resource | Status                    |
| ------------------- | ------------------------- |
| **QBCore**          | ✅ Integrated and verified |
| **Qbox**            | ✅ Integrated and verified |
| **ESX**             | 🚫 Not implemented        |
| **ox_inventory**    | Required                  |
| **ox_lib**          | Required                  |
| **ox_target**       | Required                  |
| {.dense}            |                           |

---

## Official Links

* [Apocalypse Roulette Product Page](https://bigdaddyscripts.com/Products/View/3197/Apocalypse-Roulette)
* [Apocalypse Roulette Documentation](https://wiki.bigdaddyscripts.com/Documentation/Apocalypse-Roulette/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
