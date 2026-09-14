---
title: npwd
description: Framework-agnostic FiveM phone resource built with React and TypeScript, with documented QBCore and ESX integrations.
published: true
date: 2026-09-14T02:11:05.715Z
tags: esx, phone, qbcore, script
editor: markdown
dateCreated: 2026-09-14T02:11:05.715Z
---

# npwd [![](https://badges.5metrics.dev/npwd/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/npwd)

Framework-agnostic FiveM phone resource built with React and TypeScript.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field                 | Information                      |
| --------------------- | -------------------------------- |
| **Name**              | `npwd`                           |
| **Project**           | NPWD                             |
| **Creator**           | Project Error                    |
| **Type**              | Script                           |
| **Category**          | Phone                            |
| **Game**              | FiveM                            |
| **License**           | CC BY-NC-SA 4.0                  |
| **Framework Support** | QBCore, ESX, custom integrations |
| {.dense}              |                                  |

---

## Resource Details {.tabset}

### Overview

NPWD is a FiveM phone written with React and TypeScript.

The project is designed to be framework agnostic. Its official documentation specifically describes integration with QBCore, ESX, and custom frameworks.

### Requirements

For full functionality, the installation documentation lists:

* `screenshot-basic`
* `pma-voice`

The project standardizes `pma-voice` as its supported phone voice system.

### Development

The repository is structured as a monorepo containing the phone UI, FiveM game scripts, database code, configuration, logging, types, hooks, and other packages.

---

## Installation

### Installation Checklist

* [ ] Download an official NPWD release
* [ ] Install `screenshot-basic`
* [ ] Install `pma-voice`
* [ ] Configure your framework integration
* [ ] Configure database settings
* [ ] Start dependencies before `npwd`
* [ ] Start `npwd`
* [ ] Test phone calls, media, and framework integration

### Resource Order

```cfg
ensure screenshot-basic
ensure pma-voice
ensure npwd
```

> Use an official release and follow the current installation documentation for database and framework-specific setup.
> {.is-info}

---

## Compatibility

| Item                  | Information                          |
| --------------------- | ------------------------------------ |
| **Game**              | FiveM                                |
| **QBCore**            | Supported integration                |
| **ESX**               | Supported integration                |
| **Custom frameworks** | Supported through integration system |
| **Voice**             | `pma-voice`                          |
| **Screenshots**       | `screenshot-basic`                   |
| **Resource name**     | `npwd`                               |
| {.dense}              |                                      |

---

## Links

* [Official GitHub Repository](https://github.com/project-error/npwd)
* [Official Project Error Documentation](https://projecterror.dev/docs/npwd/)

---

## Credits

Created and maintained by **Project Error** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
