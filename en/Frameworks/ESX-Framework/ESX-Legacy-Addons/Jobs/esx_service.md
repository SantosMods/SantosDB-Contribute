---
title: esx_service
description: ESX addon that provides on-duty and off-duty switching for job-based services such as police, ambulance, and taxi.
published: true
date: 2026-10-16T12:00:00.000Z
tags: script, esx, free, github, jobs
editor: markdown
dateCreated: 2026-10-16T12:00:00.000Z
---

# esx_service [![](https://badges.5metrics.dev/esx_service/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/esx_service)

ESX addon that provides on-duty and off-duty switching for job-based services such as police, ambulance, and taxi.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field              | Information   |
| ------------------ | ------------- |
| **Name**           | `esx_service` |
| **Creator**        | ESX Framework |
| **Type**           | Script        |
| **Category**       | Duty system   |
| **Game**           | FiveM         |
| **Price**          | Free          |
| **License**        | GPL-3.0-only  |
| **Framework**      | ESX Legacy    |
| **Version**        | `1.0`         |
| **Legacy Version** | `1.16.0`      |
| **Source**         | GitHub        |
| {.dense}           |               |

---

## Resource Details {.tabset}

### Overview

`esx_service` is a basic duty system. Other resources use it to let players switch on and off duty for a service.

### Requirements

* `es_extended`
* `esx_lib`

---

## Installation

### Installation Checklist

* [ ] Install and configure ESX
* [ ] Download `esx_service` from the official ESX repository
* [ ] Place `esx_service` in your server resources
* [ ] Start `esx_service` before resources that use it
* [ ] Check the server console for errors

### Resource Order

```cfg
ensure es_extended
ensure esx_service
```

---

## Usage

Enable service:

```lua
ESX.TriggerServerCallback('esx_service:enableService', function(canTakeService, maxInService, inServiceCount)
    if canTakeService then
        ESX.ShowNotification('You enabled service')
    end
end, 'taxi')
```

Disable service:

```lua
TriggerServerEvent('esx_service:disableService', 'taxi')
```

---

## Links

* [Official Documentation](https://docs.esx-framework.org/en/esx_addons/esx_service)
* [Official ESX-Legacy-Addons Repository](https://github.com/esx-framework/ESX-Legacy-Addons)
* [esx_service Source](https://github.com/esx-framework/ESX-Legacy-Addons/tree/main/%5Besx_addons%5D/esx_service)
* [ESX Framework](https://www.esx-framework.org/)

---

## Credits

Created and maintained through the **ESX Framework** project and its contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.