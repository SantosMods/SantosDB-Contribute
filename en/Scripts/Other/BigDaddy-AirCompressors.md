---
title: BigDaddy-AirCompressors
description: Lets players use in-world air compressor props to check tire pressure and refill or repair vehicle tires.
published: true
date: 2026-09-13T18:02:15.560Z
tags: qbcore, qbox, script, vehicle-repair
editor: markdown
dateCreated: 2026-09-13T15:38:50.059Z
---

# Air Compressors [![](https://badges.5metrics.dev/BigDaddy-AirCompressors/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-AirCompressors)

Air Compressors lets players use in-world compressor props to check tire pressure and refill vehicle tires.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                      | Information               |
| -------------------------- | ------------------------- |
| **Name**                   | `Air Compressors`         |
| **Resource Folder**        | `BigDaddy-AirCompressors` |
| **Creator**                | Big Daddy Scripts         |
| **Game**                   | FiveM                     |
| **Type**                   | Script                    |
| **Category**               | Vehicles                  |
| **Price**                  | $5.00 USD                 |
| **QBCore / Qbox**          | ✔ Stand-Alone compatible  |
| **ESX**                    | ✔ Stand-Alone compatible  |
| **BigDaddy-VehicleDamage** | Optional integration      |
| **Targeting**              | `ox_target`, `qb_target`  |
| **Runtime**                | CFX Mono V2               |
| {.dense}                   |                           |

> The Big Daddy Scripts product catalog and product detail page have shown different patch versions for Air Compressors. Check the official product page for the current version before installation.
> {.is-info}

---

## Resource Details {.tabset}

### Overview

Air Compressors makes supported air compressor objects usable for vehicle tire maintenance.

Players can take a hose from a compressor, move to a vehicle tire, and refill it. The script can also report the tire's actual pressure or health.

Existing base-game compressor props are supported, and additional compressor models can be configured.

### Features

* Refill and repair vehicle tires
* Check tire pressure or tire health
* Uses in-world compressor objects
* Networked hoses and objects
* Configurable compressor models
* Optional compressor usage costs
* Optional BigDaddy-VehicleDamage integration
* `ox_target` support
* `qb_target` support

### Vehicle Damage Integration

Air Compressors integrates with Big Daddy Scripts Vehicle Damage.

The integration is optional. Air Compressors can run without Vehicle Damage.

When both are installed, tires affected by Vehicle Damage can be refilled using Air Compressors.

---

## Installation

### Installation Checklist

* [ ] Download the resource from Big Daddy Scripts.
* [ ] Extract `BigDaddy-AirCompressors` into your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Configure money integration if required.
* [ ] Configure additional compressor props if required.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-AirCompressors
```

> Do not rename `BigDaddy-AirCompressors`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration {.tabset}

### settings.ini

| Setting          | Default      | Description                                                                |
| ---------------- | ------------ | -------------------------------------------------------------------------- |
| `key1`           | `none`       | Big Daddy Scripts product key                                              |
| `useMoney`       | `true`       | Enables money-framework integration when `server.lua` is configured        |
| `DisplayPrompts` | `true`       | Controls on-screen prompts                                                 |
| `HoseCanBreak`   | `true`       | Allows the hose to break when the player moves too far from the compressor |
| `[locales]`      | configurable | Language used for prompts and messages                                     |
| {.dense}         |              |                                                                            |

### Compressors.json

`Compressors.json` contains the compressor prop definitions used by the script.

A compressor entry can define:

* Object model
* Hose attachment offset
* Usage cost

The official documentation notes that most configured compressors have a cost of `0`, while compressors at gas stations can be assigned a cost when money integration is enabled.

---

## Interaction

### Commands

When targeting is not used:

```text
/checkair
```

Use `/checkair` near a tire to check its pressure or health.

```text
/airpump
```

Use `/airpump` near a compressor to take the hose.

Move to a tire and follow the prompts to refill it. Return to the compressor and use `/airpump` again to put the hose away, or press `X`.

### Targeting

When `ox_target` or `qb_target` is installed, Air Compressors automatically uses the targeting resource for compressor and tire interaction.

---

## Compatibility

| Platform / Resource        | Status                               |
| -------------------------- | ------------------------------------ |
| **Stand-Alone**            | Supported                            |
| **QBCore**                 | ✔ Verified Stand-Alone compatibility |
| **Qbox**                   | ✔ Verified Stand-Alone compatibility |
| **ESX**                    | ✔ Verified Stand-Alone compatibility |
| **ox_target**              | Supported                            |
| **qb_target**              | Supported                            |
| **BigDaddy-VehicleDamage** | Optional integration                 |
| {.dense}                   |                                      |

The current compatibility table marks QBCore/Qbox and ESX with **✔**. Big Daddy Scripts defines this as verified Stand-Alone compatibility rather than framework implementation.

---

## Official Links

* [Air Compressors Product Page](https://bigdaddyscripts.com/Products/View/2911/Air-Compressors)
* [Air Compressors Documentation](https://wiki.bigdaddyscripts.com/Documentation/Air-Compressors/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
