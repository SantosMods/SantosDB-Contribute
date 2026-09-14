---
title: cd_easytime
description: FiveM time and weather management resource with an administrative UI for changing server weather and time.
published: true
date: 2026-09-14T23:52:29.588Z
tags: script, standalone, weather-control, time
editor: markdown
dateCreated: 2026-09-14T23:52:29.588Z
---

# cd_easytime [![](https://badges.5metrics.dev/cd_easytime/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/cd_easytime)

FiveM time and weather management resource with an administrative UI for changing server weather and time.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

## Resource Information

| Field              | Information               |
| ------------------ | ------------------------- |
| **Name**           | `cd_easytime`             |
| **Project**        | Easytime                  |
| **Repository**     | `dsheedes/cd_easytime`    |
| **Type**           | Script                    |
| **Category**       | Time and Weather          |
| **Game**           | FiveM                     |
| **Base operation** | Standalone                |
| **License**        | Custom repository license |
| {.dense}           |                           |

## Resource Details {.tabset}

### Overview

Easytime provides a UI for FiveM server administrators to control server time and weather.

The default command for opening the interface is:

```text
/easytime
```

### Framework

The official README describes Easytime as standalone while also instructing server owners to configure:

```lua
Config.Framework
```

Use the framework value documented for your server setup.

### Conflicts

> Easytime can conflict with other resources that control time or weather, including vMenu and vSync.
> {.is-warning}

Avoid running multiple resources that synchronize the same time and weather state.

## Installation

### Installation Checklist

* [ ] Download `cd_easytime` from the official repository
* [ ] Place it in your resources directory
* [ ] Review the current CodeSign documentation
* [ ] Configure `Config.Framework`
* [ ] Disable conflicting time and weather synchronization
* [ ] Start `cd_easytime`
* [ ] Test `/easytime`

```cfg
ensure cd_easytime
```

## Usage

Open the administrative interface with the documented default command:

```text
/easytime
```

## Links

* [Official GitHub Repository](https://github.com/dsheedes/cd_easytime)
* [Official CodeSign Documentation](https://docs.codesign.pro/free-scripts/easytime-time-and-weather-management)

## Credits

The repository is maintained under **dsheedes** and links to official **CodeSign** documentation.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
