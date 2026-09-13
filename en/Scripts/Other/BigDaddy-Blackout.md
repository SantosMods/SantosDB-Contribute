---
title: BigDaddy-Blackout
description: Controls statewide power blackouts with permanent or randomized modes, ACE permissions, optional EAS integration, and server events for other resources.
published: true
date: 2026-09-13T18:03:40.738Z
tags: blackout, script, standalone, weather-control
editor: markdown
dateCreated: 2026-09-13T17:58:05.207Z
---

# Blackout [![](https://badges.5metrics.dev/BigDaddy-Blackout/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/BigDaddy-Blackout)

Blackout controls statewide power outages with permanent and randomized blackout modes.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field               | Information              |
| ------------------- | ------------------------ |
| **Name**            | `Blackout`               |
| **Resource Folder** | `BigDaddy-Blackout`      |
| **Creator**         | Big Daddy Scripts        |
| **Game**            | FiveM                    |
| **Type**            | Script                   |
| **Category**        | Environment              |
| **Version**         | `v1.4.2`                 |
| **Price**           | $8.00 USD                |
| **QBCore / Qbox**   | ✔ Stand-Alone compatible |
| **ESX**             | ✔ Stand-Alone compatible |
| **ACE Permissions** | Supported                |
| **BigDaddy-EAS**    | Optional integration     |
| {.dense}            |                          |

---

## Resource Details {.tabset}

### Overview

Blackout can disable environmental power across the state.

It supports a persistent blackout mode and a random mode that switches the power on and off using configurable timing.

### Features

* Statewide blackout
* Permanent blackout mode
* Random blackout mode
* Configurable random timing
* ACE-restricted commands
* Optional BigDaddy-EAS announcements
* Server events for integrations
* Auto-start blackout options

> Blackout does not disable vehicle headlights or emergency vehicle lights.
> {.is-info}

---

## Compatibility Warning

> Disable blackout and dynamic weather functions in vMenu, QBCore weather resources, or any other resource controlling the same systems. Competing resources can cause the blackout to flicker instead of remaining active.
> {.is-warning}

This conflict is specifically documented by Big Daddy Scripts.

---

## Installation

### Installation Checklist

* [ ] Disable conflicting blackout controls.
* [ ] Disable conflicting dynamic weather controls where required.
* [ ] Download Blackout from Big Daddy Scripts.
* [ ] Place `BigDaddy-Blackout` in your resources folder.
* [ ] Keep the folder name unchanged.
* [ ] Add your product key to `settings.ini`.
* [ ] Configure ACE permissions if required.
* [ ] Configure BigDaddy-EAS integration if used.
* [ ] Add the resource to `server.cfg`.
* [ ] Restart the server.

```cfg
start BigDaddy-Blackout
```

> Do not rename `BigDaddy-Blackout`. The official documentation states that changing the folder name prevents the resource from functioning correctly.
> {.is-danger}

---

## Configuration

| Setting                     | Default      | Description                                                    |
| --------------------------- | ------------ | -------------------------------------------------------------- |
| `key1`                      | `none`       | Big Daddy Scripts product key                                  |
| `useAcePermissions`         | `true`       | Restricts blackout commands with ACE permissions               |
| `acePermission`             | `Command`    | ACE permission required for commands                           |
| `useEAS`                    | `true`       | Sends a server-wide EAS message when BigDaddy-EAS is installed |
| `EASMessageTitle`           | configurable | EAS message title                                              |
| `EASMessage`                | configurable | EAS message body                                               |
| `alwaysBlackout`            | `false`      | Starts a permanent blackout on server start                    |
| `alwaysRandomBlackout`      | `false`      | Starts random blackout mode on server start                    |
| `minRandomBlackoutDuration` | `2`          | Minimum random duration and interval in minutes                |
| `maxRandomBlackoutDuration` | `16`         | Maximum random duration and interval in minutes                |
| {.dense}                    |              |                                                                |

---

## Commands

Start a permanent blackout:

```text
/startblackout
```

Start random blackout mode:

```text
/startblackoutrandom
```

Stop either mode:

```text
/endblackout
```

The random mode repeatedly selects blackout and powered intervals between the configured minimum and maximum durations.

---

## Server Events

Other resources can control Blackout through these server events.

### Start Blackout

```text
BigDaddy-Blackout:TriggerBlackout
```

Equivalent to:

```text
/startblackout
```

### Start Random Blackouts

```text
BigDaddy-Blackout:TriggerBlackoutRandom
```

Equivalent to:

```text
/startblackoutrandom
```

### End Blackout

```text
BigDaddy-Blackout:EndBlackout
```

Equivalent to:

```text
/endblackout
```

---

## BigDaddy-EAS Integration

When `useEAS=true` and BigDaddy-EAS is installed, Blackout can issue a server-wide EAS announcement when a blackout begins.

The title and body are configurable with:

```text
EASMessageTitle
EASMessage
```

BigDaddy-EAS is optional.

---

## Compatibility

| Platform / Resource                    | Status                               |
| -------------------------------------- | ------------------------------------ |
| **Stand-Alone**                        | Supported                            |
| **QBCore**                             | ✔ Verified Stand-Alone compatibility |
| **Qbox**                               | ✔ Verified Stand-Alone compatibility |
| **ESX**                                | ✔ Verified Stand-Alone compatibility |
| **ACE Permissions**                    | Supported                            |
| **BigDaddy-EAS**                       | Optional integration                 |
| **Other blackout/weather controllers** | Must be disabled when conflicting    |
| {.dense}                               |                                      |

---

## Official Links

* [Blackout Product Page](https://bigdaddyscripts.com/Products/View/1949/Blackout)
* [Blackout Documentation](https://wiki.bigdaddyscripts.com/Documentation/Blackout/)
* [Compatibility Checks](https://wiki.bigdaddyscripts.com/Documentation/Compatibility/)
* [Big Daddy Scripts](https://bigdaddyscripts.com/)

---

## Credits

Created by **Big Daddy Scripts**, a division of **I CAN MAKE THAT, INC.**, and applicable project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
