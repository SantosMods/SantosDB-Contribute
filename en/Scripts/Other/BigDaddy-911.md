---
title: BigDaddy-911
description: Stand-alone emergency call script with configurable emergency numbers, map blips, Discord logging, BigDaddy-Chat integration, and a client export.
published: true
date: 2026-09-13T18:00:48.823Z
tags: emergency-services, qbcore, qbox, script
editor: markdown
dateCreated: 2026-09-13T15:36:05.387Z
---

# 911 [![](https://badges.5metrics.dev/BigDaddy-911/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-911)

911 provides a configurable emergency call command with map blips, optional Discord logging, and an export for other scripts.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `911`                    |
| **Resource Folder** | `BigDaddy-911`           |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Script                   |
| **Category**        | Emergency Services       |
| **Version**         | `v1.2.2`                 |
| **Price**           | $5.00 USD                |
| **Dependencies**    | None                     |
| **QBCore / Qbox**   | ✔ Stand-Alone compatible |
| **ESX**             | ✔ Stand-Alone compatible |
| **Runtime**         | CFX Mono V2              |
| {.dense}            |                          |

> A **✔** in Big Daddy Scripts' compatibility table means the Stand-Alone script is verified working with the framework. It does not mean the script is integrated with that framework.
> {.is-info}

---

## Resource Details {.tabset}

### Overview

911 provides an emergency call system for servers without existing 911 or CAD integration.

Players submit an emergency call through a configurable command. The script can display the call globally, create a temporary map blip, and send the call to Discord through a webhook.

The default emergency number is `911`, but you can configure another number such as `999` or `000`.

### Features

* Configurable emergency call number
* Temporary map blips for calls
* Configurable blip duration and radius
* Optional Discord webhook logging
* Optional nearest-postal integration
* BigDaddy-Chat integration
* Client export for other resources

### BigDaddy-Chat

BigDaddy-Chat integration is supported but not required.

When BigDaddy-Chat is installed, emergency calls display as LEO messages. Other chat resources receive the calls as system messages.

---

## Installation

### Installation Checklist

* [ ] Download the purchased ZIP from Big Daddy Scripts.
* [ ] Extract `BigDaddy-911` into your resources folder.
* [ ] Keep the resource folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.
* [ ] Check the server and client consoles.

Add:

```cfg
start BigDaddy-911
```

> Do not rename `BigDaddy-911`. The official documentation states that changing the resource folder name prevents the script from functioning correctly.
> {.is-danger}

---

## Configuration

911 uses `settings.ini`.

| Setting               | Default | Description                                                      |
| --------------------- | ------- | ---------------------------------------------------------------- |
| `key1`                | `none`  | Big Daddy Scripts product key                                    |
| `webhookUrl`          | blank   | Discord webhook for emergency messages; leave blank to disable   |
| `blipTime`            | `180`   | Number of seconds the call blip remains visible; `0` disables it |
| `blipRadius`          | `75.0`  | Blip radius in meters                                            |
| `emergencyNumber`     | `911`   | Number used for the emergency command                            |
| `nearestPostalScript` | blank   | Nearest-postal resource used in emergency messages               |
| `nearestPostalExport` | blank   | Export used by the configured postal resource                    |
| {.dense}              |         |                                                                  |

---

## Usage

Use the configured emergency number followed by the call description.

With the default configuration:

```text
/911 description
```

The call is posted globally. When enabled, the script also creates a temporary map blip and sends the message through the configured Discord webhook.

---

## Developer Export

### Client Export

```lua
exports['BigDaddy-911']:EmergencyCall(Message, X, Y, Z, Name)
```

| Argument  | Type   |
| --------- | ------ |
| `Message` | string |
| `X`       | float  |
| `Y`       | float  |
| `Z`       | float  |
| `Name`    | string |
| {.dense}  |        |

The export does not document a return value.

---

## Compatibility

| Platform          | Status                               |
| ----------------- | ------------------------------------ |
| **Stand-Alone**   | Supported                            |
| **QBCore**        | ✔ Verified Stand-Alone compatibility |
| **Qbox**          | ✔ Verified Stand-Alone compatibility |
| **ESX**           | ✔ Verified Stand-Alone compatibility |
| **BigDaddy-Chat** | Integrated, optional                 |
| {.dense}          |                                      |

The script uses the CFX Mono V2 runtime. Big Daddy Scripts states that build `2944` cannot load this runtime and requires `3095+`. Big Daddy Scripts tests on and recommends build `3095`.

---

## Official Links

* [911 Product Page](https://bigdaddyscripts.com/Products/View/2222/911)
* [911 Documentation](https://wiki.bigdaddyscripts.com/Documentation/911/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
