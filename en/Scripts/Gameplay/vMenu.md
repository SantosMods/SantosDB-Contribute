---
title: vMenu
description: Standalone FiveM server menu with permission-controlled player, vehicle, world, and administrative functionality.
published: true
date: 2026-09-14T02:12:06.962Z
tags: admin, menus, script, standalone
editor: markdown
dateCreated: 2026-09-14T02:12:06.962Z
---

# vMenu [![](https://badges.5metrics.dev/vMenu/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/vMenu)

Standalone FiveM server menu with permission-controlled player, vehicle, world, and administrative functionality.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information |
| ------------- | ----------- |
| **Name**      | `vMenu`     |
| **Creator**   | Vespura     |
| **Type**      | Script      |
| **Category**  | Server Menu |
| **Game**      | FiveM       |
| **Framework** | Standalone  |
| {.dense}      |             |

> The official documentation now separates **vMenu for FiveM Legacy** and **vMenu for FiveM Enhanced**. This page covers the established `vMenu` resource for FiveM Legacy. `vMenu.Enhanced` has different installation and resource-name requirements.
> {.is-info}

---

## Resource Details {.tabset}

### Overview

`vMenu` provides a configurable server-side menu for FiveM.

Access to menus and actions can be controlled through FiveM ACE permissions and principals.

### Permissions

vMenu permissions use ACEs such as:

```text
vMenu.PlayerOptions.Menu
vMenu.NoClip
vMenu.Staff
```

Groups are configured with FiveM principals.

Example:

```cfg
add_principal identifier.steam:110000101234567 group.admin
```

### Configuration

Legacy vMenu uses convars for configuration.

Example:

```cfg
setr vmenu_use_permissions true
```

The supplied `permissions.cfg` can contain both permissions and configuration options.

---

## Installation

### Installation Checklist

* [ ] Download vMenu from the official source
* [ ] Place `vMenu` in your resources folder
* [ ] Configure `permissions.cfg`
* [ ] Add the permissions file to `server.cfg`
* [ ] Start `vMenu`
* [ ] Fully restart the server after permission changes
* [ ] Test access with each permission group

### Resource Order

Example Legacy configuration:

```cfg
exec resources/vMenu/config/permissions.cfg
ensure vMenu
```

> `permissions.cfg` is executed by the FiveM server. vMenu does not directly read the file itself.
> {.is-info}

> Permission-file changes require a server restart. Restarting only the `vMenu` resource does not reload those ACE commands.
> {.is-warning}

---

## Known Issues

The official FAQ notes that running multiple weather or time synchronization resources can cause sky flickering.

Disable overlapping weather or time systems, or disable the corresponding vMenu synchronization features.

---

## Links

* [Official Documentation](https://docs.vespura.com/vmenu/)
* [Legacy Documentation](https://docs.vespura.com/vmenu/legacy/)
* [Permissions Documentation](https://docs.vespura.com/vmenu/legacy/permissions/)

---

## Credits

Created and maintained by **Vespura** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
