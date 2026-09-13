---
title: BigDaddy-Airbags
description: Adds collision-triggered airbags with configurable vehicle exemptions, reset controls, and an option to disable vehicles after deployment.
published: true
date: 2026-09-13T18:01:49.657Z
tags: qbcore, qbox, script, vehicle-safety
editor: markdown
dateCreated: 2026-09-13T15:40:45.120Z
---

# Airbags [![](https://badges.5metrics.dev/BigDaddy-Airbags/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-Airbags)

Airbags adds collision-triggered airbags to FiveM vehicles with configurable vehicle exemptions and deployment behavior.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `Airbags`                |
| **Resource Folder** | `BigDaddy-Airbags`       |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Script                   |
| **Category**        | Vehicles                 |
| **Price**           | $10.00 USD               |
| **Dependencies**    | None                     |
| **QBCore / Qbox**   | ✔ Stand-Alone compatible |
| **ESX**             | ✔ Stand-Alone compatible |
| **Runtime**         | CFX Mono V2              |
| {.dense}            |                          |

> Airbag functionality is already included with Big Daddy Scripts Speedometer+. Do not install the separate Airbags resource when you already use that functionality through `BigDaddy-Speedometer`.
> {.is-danger}

---

## Resource Details {.tabset}

### Overview

Airbags deploy when a supported vehicle experiences a collision.

The script provides configuration for which vehicles can use airbags and how the vehicle behaves after deployment.

Players can reset deployed airbags with configurable controls unless vehicle disabling is enabled.

### Features

* Collision-triggered airbag deployment
* Custom airbag objects
* Configurable vehicle classes
* Configurable vehicle model exemptions
* Optional emergency vehicle exemption
* Configurable reset controls
* Optional vehicle disabling after deployment
* Configurable visible prompts

---

## Installation

### Installation Checklist

* [ ] Confirm you do not already use the Airbags functionality included with Speedometer+.
* [ ] Download Airbags from Big Daddy Scripts.
* [ ] Extract `BigDaddy-Airbags` into your resources folder.
* [ ] Keep the resource folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Configure vehicle exemptions.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-Airbags
```

> Do not rename `BigDaddy-Airbags`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration

Airbags uses `settings.ini`.

| Setting                             | Default               | Description                                        |
| ----------------------------------- | --------------------- | -------------------------------------------------- |
| `key1`                              | `none`                | Big Daddy Scripts product key                      |
| `showPropts`                        | `true`                | Controls whether reset prompts are displayed       |
| `disableVehicleWithAirbagsDeployed` | `false`               | Disables the vehicle after deployment when enabled |
| `airbags`                           | `true`                | Enables airbag functionality                       |
| `classExempt`                       | `8,13,14,15,16,21`    | Vehicle classes excluded from airbags              |
| `modelExempt`                       | `caddy,caddy2,caddy3` | Vehicle models excluded from airbags               |
| `airbagSecondaryKey`                | `LALT`                | Secondary reset key                                |
| `airbagKey`                         | `X`                   | Primary reset key                                  |
| `exemptEmergency`                   | `false`               | Excludes emergency vehicles when enabled           |
| `[locales]`                         | configurable          | Visible prompt language                            |
| {.dense}                            |                       |                                                    |

> `showPropts` is preserved exactly as documented by Big Daddy Scripts.
> {.is-info}

### Vehicle Disabling

When:

```ini
disableVehicleWithAirbagsDeployed=true
```

the vehicle no longer runs after its airbags deploy.

The official documentation also notes that this disables the ability to reset the airbags. The vehicle remains disabled after deployment.

---

## Compatibility

| Platform         | Status                                |
| ---------------- | ------------------------------------- |
| **Stand-Alone**  | Supported                             |
| **QBCore**       | ✔ Verified Stand-Alone compatibility  |
| **Qbox**         | ✔ Verified Stand-Alone compatibility  |
| **ESX**          | ✔ Verified Stand-Alone compatibility  |
| **Speedometer+** | Airbag functionality already included |
| {.dense}         |                                       |

Airbags has no required dependencies.

The script uses CFX Mono V2. Big Daddy Scripts requires game build `3095+` for this runtime and tests on build `3095`.

---

## Known Conflicts

### Speedometer+

Speedometer+ already contains the same airbag functionality.

Do not purchase or run the separate Airbags resource solely to add airbags when you already use the included Speedometer+ implementation.

---

## Official Links

* [Airbags Product Page](https://bigdaddyscripts.com/Products/View/2079/Airbags)
* [Airbags Documentation](https://wiki.bigdaddyscripts.com/Documentation/Airbags/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
