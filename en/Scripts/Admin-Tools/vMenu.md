---
title: vMenu
description: Standalone FiveM server menu with permission-controlled player, vehicle, world, and administrative functionality.
published: true
date: 2026-09-16T00:39:48.211Z
tags: admin, menus, script, standalone
editor: markdown
dateCreated: 2026-09-14T02:12:06.962Z
---

# vMenu [![](https://badges.5metrics.dev/vMenu/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/vMenu)

vMenu is a server-sided trainer/menu for FiveM servers. It provides configurable player, vehicle, world, server administration, and customization tools with ACE permission support.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

> **Legacy status:** The creator's documentation identifies this version of vMenu as **vMenu (Legacy)**. It is no longer actively supported. It may receive small updates from community pull requests or FiveM content updates while work continues on vMenu Enhanced.
> {.is-warning}

---

## Resource Information

| Field               | Information                                     |
| ------------------- | ----------------------------------------------- |
| **Name**            | `vMenu`                                         |
| **Creator**         | Tom Grobbe / Vespura                            |
| **Type**            | FiveM server resource                           |
| **Category**        | Menu / Administration                           |
| **Game**            | FiveM                                           |
| **Framework**       | Standalone                                      |
| **Permissions**     | FiveM ACE / Principal permissions               |
| **Menu API**        | MenuAPI                                         |
| **Configuration**   | ConVars, ACE permissions, JSON configuration    |
| **Price**           | Free download from the official GitHub releases |
| **Source**          | Official GitHub repository                      |
| **License**         | Custom project license                          |
| **Support Status**  | Legacy / limited maintenance                    |
| **Resource Folder** | `vMenu`                                         |
| **Manifest**        | `fxmanifest.lua`                                |
| {.dense}            |                                                 |

> The resource folder must be named exactly `vMenu`. The official installation documentation states that the name is case-sensitive and that changing it will break the resource.
> {.is-warning}

---

## Resource Details {.tabset}

### Overview

vMenu provides a server-controlled menu for FiveM. Server owners can control access to menus and individual actions through FiveM's ACE permission system.

The project describes vMenu as a server-sided trainer/menu. Its permission system allows server owners to decide which players or groups can access specific functionality.

vMenu includes functionality covering areas such as:

* Player options
* Vehicle options
* Vehicle spawning
* Saved vehicles
* Online player management
* Weapon options
* Weapon loadouts
* Recording options
* Miscellaneous settings
* Player appearance
* MP character customization
* Teleport locations
* Server-defined map blips
* Addon vehicles
* Addon peds
* Addon weapons
* Addon weapon components
* Custom tattoos
* Vehicle extra labels
* Model restrictions
* Administrative actions

Exact access depends on the server's ACE configuration.

### Architecture

vMenu contains client and server components and uses MenuAPI for its menu system.

Starting with vMenu v2.1.0, the project uses **MenuAPI (MAPI)**, a custom menu API created for vMenu.

Versions v2.0.0 and earlier used a modified NativeUI implementation.

The repository contains separate areas including:

```text
vMenu/
vMenuServer/
SharedClasses/
dependencies/
assets/
docs/
```

Server operators normally install a packaged release rather than manually assembling these repository directories.

### Framework Support

vMenu does not require QBCore, Qbox, ESX, or another roleplay framework for its documented permission system.

Its access control uses FiveM ACE permissions and principals.

This makes the resource usable independently of a roleplay framework, but it does **not** imply automatic integration with framework jobs, groups, permissions, characters, inventories, or other framework systems.

### Dependencies

The official installation process does not instruct server owners to install QBCore, Qbox, ESX, `ox_lib`, `oxmysql`, or another external roleplay framework dependency.

Use an up-to-date FXServer artifact before installing vMenu.

---

## Core Features

### Permission-Controlled Menus

vMenu uses FiveM ACE permissions.

A server owner can grant access to an entire submenu or grant individual actions.

Common permission patterns include:

```text
vMenu.PlayerOptions.Menu
vMenu.PlayerOptions.All
```

`.Menu` controls whether the submenu can be opened.

`.All` grants all supported permissions within that menu.

> Do not grant a menu's `.All` permission if you intend to restrict individual options inside that menu. `.All` overrides the individual option restrictions.
> {.is-warning}

### Principals

FiveM principals act as permission groups.

You can create groups such as:

```text
group.admin
group.moderator
group.owner
group.vip
```

A player can then be assigned to a principal.

Example:

```cfg
add_principal identifier.steam:110000101234567 group.admin
```

The group can receive ACE permissions instead of assigning every permission directly to every player.

### Principal Inheritance

Principals can be assigned to other principals, allowing group inheritance.

This lets a server build permission structures without duplicating every ACE entry across every staff role.

### Everyone Permissions

`builtin.everyone` applies to every player.

> Permissions granted to `builtin.everyone` also apply to administrators, moderators, and other groups. It means everyone.
> {.is-info}

---

## Installation

### Before You Install

* [ ] Update your FXServer artifacts
* [ ] Download an official packaged vMenu release
* [ ] Back up an existing vMenu configuration if updating
* [ ] Confirm the destination folder will be named exactly `vMenu`
* [ ] Review `permissions.cfg`
* [ ] Review the official documentation for the version you install

> Download a release package from the project's official GitHub Releases page. Do not use an unknown mirror or reupload.
> {.is-info}

### Installation Checklist

* [ ] Download `vMenu-<version>.zip` from the official GitHub Releases page
* [ ] Extract the archive
* [ ] Copy the resource to your server resources directory
* [ ] Confirm `fxmanifest.lua` is directly inside the `vMenu` resource
* [ ] Configure `permissions.cfg`
* [ ] Execute the permissions configuration before starting vMenu
* [ ] Add `ensure vMenu`
* [ ] Restart the server
* [ ] Join and test menu access
* [ ] Check permissions for normal players and staff separately

### Resource Structure

The expected installation location is:

```text
resources/vMenu/
```

The manifest must resolve as:

```text
resources/vMenu/fxmanifest.lua
```

Do **not** install it as:

```text
resources/vMenu/vMenu/
```

The resource folder must be named:

```text
vMenu
```

### server.cfg

The official installation documentation uses:

```cfg
exec @vMenu/config/permissions.cfg
ensure vMenu
```

The order matters.

Execute `permissions.cfg` **before** `ensure vMenu`.

> vMenu does not directly read `permissions.cfg`. FXServer executes the commands in that file. vMenu then asks the server whether a player has the required ACE permission.
> {.is-info}

---

## Updating vMenu

When updating an existing installation, the official documentation instructs server owners to replace the resource files while preserving their configuration.

Keep:

```text
permissions.cfg
vMenu/config/
```

Replace the other files with the files supplied by the new release.

> Back up your complete `vMenu` resource before updating. Review the release changelog for version-specific migration instructions.
> {.is-warning}

If upgrading from a version older than v3.3.0 and saved bans must be retained, consult the official changelog before updating.

---

## Permissions

### Permission Concepts

vMenu permissions use two FiveM concepts:

| vMenu Term             | FiveM Concept      | Purpose                                                |
| ---------------------- | ------------------ | ------------------------------------------------------ |
| **Ace**                | Permission         | Grants access to an action or menu                     |
| **Principal**          | Group / identity   | Receives ACE permissions or inherits another principal |
| **`.Menu`**            | Menu ACE           | Allows the submenu to be opened                        |
| **`.All`**             | Broad menu ACE     | Grants supported actions inside that menu              |
| **`builtin.everyone`** | Built-in principal | Applies to every connected player                      |
| {.dense}               |                    |                                                        |

### Basic Group Example

```cfg
add_principal identifier.steam:110000101234567 group.admin
```

Permissions can then be assigned to `group.admin`.

Conceptually:

```cfg
add_ace group.admin vMenu.PlayerOptions.Menu allow
```

Use the official permission reference for the exact ACE names you want to grant.

### Do Not Use `deny` as a Normal Restriction Method

The official permissions guide warns against setting unwanted vMenu permissions to `deny`.

Instead, remove or comment out the ACE grant.

Example:

```cfg
# add_ace group.example vMenu.Example.Permission allow
```

> If a group receives a broad `.All` permission, attempting to selectively restrict a child permission can produce results different from what you expect. Build permission groups from explicit grants when fine-grained access matters.
> {.is-warning}

### Permission Changes Require a Server Restart

Changes to `permissions.cfg` require a server restart because the configuration file is executed during server startup.

Restarting only the vMenu resource does not re-execute the permissions file.

Use this workflow:

* [ ] Stop the server
* [ ] Edit the active `permissions.cfg`
* [ ] Save the file
* [ ] Start the server
* [ ] Test using the affected player or group

### Verify the Correct permissions.cfg

Do not accidentally edit a copy that FXServer never executes.

If your configuration uses:

```cfg
exec @vMenu/config/permissions.cfg
```

edit the file used by that resource path.

If you place `permissions.cfg` somewhere else, make sure the `exec` path points to that exact file.

---

## Configuration

vMenu uses ConVars for many general settings.

The documented syntax is:

```cfg
setr vmenu_option_name value
```

Configuration values can be placed in `permissions.cfg` or `server.cfg`.

When placing vMenu configuration in `server.cfg`, define it before vMenu starts.

### Permissions System

A central setting is:

```cfg
setr vmenu_use_permissions true
```

Setting `vmenu_use_permissions` to `true` enables the configured permission system.

The official configuration warns that disabling it switches to vMenu's default permission behavior and disables sensitive administration features such as banning, kicking, and unbanning.

### Staff-Only Menu

vMenu also provides a configuration option for restricting the overall menu to staff:

```cfg
setr vmenu_menu_staff_only true
```

When enabled, access depends on the corresponding `vMenu.Staff` permission.

> Review the current official configuration reference before changing ConVars. Available settings and behavior can change between releases.
> {.is-info}

---

## Configuration Files

The vMenu configuration directory contains several files for server-specific content.

```text
vMenu/config/
```

Important configuration files documented by the project include:

| File                    | Purpose                                                                     |
| ----------------------- | --------------------------------------------------------------------------- |
| `permissions.cfg`       | ConVars and ACE permission setup                                            |
| `addons.json`           | Addon vehicles, peds, weapons, weapon components, and extra blendable faces |
| `extras.json`           | Friendly labels for vehicle extras                                          |
| `locations.json`        | Teleport locations and configurable blips                                   |
| `model-whitelists.json` | Model restriction configuration                                             |
| `tattoos.json`          | Custom streamed tattoo overlays                                             |
| {.dense}                |                                                                             |

---

## addons.json

`addons.json` tells vMenu about custom content installed on the server.

It is located in:

```text
resources/vMenu/config/
```

Documented sections include:

```json
{
  "vehicles": [],
  "peds": [],
  "weapons": [],
  "weapon_components": [],
  "extra_blendable_faces": []
}
```

### Addon Vehicles

Add vehicle model spawn names to the `vehicles` array.

Example structure:

```json
{
  "vehicles": [
    "examplevehicle1",
    "examplevehicle2"
  ]
}
```

### Addon Peds

Add ped model names to the `peds` array.

```json
{
  "peds": [
    "exampleped1",
    "exampleped2"
  ]
}
```

### Addon Weapons

Add custom weapon names to the `weapons` array.

```json
{
  "weapons": [
    "WEAPON_EXAMPLE"
  ]
}
```

### Weapon Components

Custom streamed weapon components can be added under:

```json
{
  "weapon_components": [
    "COMPONENT_EXAMPLE_SCOPE",
    "COMPONENT_EXAMPLE_CLIP"
  ]
}
```

vMenu checks listed addon components against weapons and exposes compatible components.

Base-game weapon components are already handled by vMenu and do not need to be listed as addon components.

### Extra Blendable Faces

Custom blendable heads can be named using:

```json
{
  "extra_blendable_faces": [
    "Custom Head 1",
    "Custom Head 2"
  ]
}
```

Order is important.

The entries correspond to head IDs after the base-game blendable heads. Adding, removing, or reordering entries changes that mapping.

> Duplicate names in `extra_blendable_faces` are rejected. Keep every configured face name unique.
> {.is-warning}

---

## Addon Vehicle Display Names

vMenu does not provide its own vehicle-renaming configuration.

The official documentation recommends defining the vehicle's game display name through the vehicle resource.

A vehicle resource can register a display label using FiveM's `AddTextEntry`.

Example:

```lua
Citizen.CreateThread(function()
    AddTextEntry("examplecar", "Example Car")
end)
```

The model's `vehicles.meta` `<gameName>` should correspond to the vehicle model identifier used by the label registration.

This configuration belongs to the vehicle resource rather than vMenu.

---

## extras.json

`extras.json` gives vehicle extras readable menu labels.

Without custom labels, vMenu displays generic entries such as:

```text
Extra #1
Extra #2
```

A configured entry can use descriptive names.

```json
{
  "examplepolicecar": {
    "1": "Push Bar",
    "2": "Light Bar",
    "3": "Spotlight"
  }
}
```

The top-level key is the vehicle's spawn name.

The nested keys are extra IDs.

The values are display labels.

> `extras.json` only changes labels. It does not create an extra, enable an unavailable extra, or alter the vehicle model.
> {.is-info}

vMenu displays supported extras only when they exist on the current vehicle.

Invalid JSON is reported in the console.

A missing `extras.json` file is not treated as an error. vMenu falls back to its default extra labels.

---

## locations.json

`locations.json` configures custom teleport locations and map blips.

### Teleports

A teleport contains a name, coordinates, and heading.

Example structure:

```json
{
  "teleports": [
    {
      "name": "Example Location",
      "coordinates": {
        "x": 472.94,
        "y": -3035.96,
        "z": 6.2
      },
      "heading": 356.1
    }
  ]
}
```

Configured teleport locations are available through vMenu's Misc Settings area when the relevant menu access is available.

### Blips

A blip can define:

```json
{
  "blips": [
    {
      "name": "Example Blip",
      "coordinates": {
        "x": 472.94,
        "y": -3035.96,
        "z": 6.2
      },
      "spriteID": 1,
      "color": 1
    }
  ]
}
```

Use valid FiveM/GTA blip sprite and color values.

> Keep `locations.json` valid JSON. Missing commas, brackets, or braces can prevent the configuration from loading correctly.
> {.is-warning}

---

## model-whitelists.json

vMenu includes a dedicated `model-whitelists.json` configuration file for model restriction functionality.

Use the official configuration documentation for its current schema and supported whitelist categories.

Because model restrictions affect which configured models players can use, test restrictions with both normal users and privileged groups before deploying changes to a live server.

---

## tattoos.json

`tattoos.json` adds custom streamed tattoo overlays to MP Character customization.

The file is located in:

```text
resources/vMenu/config/
```

The file uses a JSON array.

A basic entry uses:

```json
[
  {
    "gender": 2,
    "name": "mytattoos_05_A",
    "collectionName": "mytattoos_overlays"
  }
]
```

### Tattoo Fields

| Field            | Required | Purpose                                |
| ---------------- | -------- | -------------------------------------- |
| `gender`         | Yes      | Selects male, female, or both          |
| `name`           | Yes      | Overlay name                           |
| `collectionName` | Yes      | Overlay collection                     |
| `zoneId`         | No       | Accepted but ignored for addon tattoos |
| `type`           | No       | Accepted but ignored for addon tattoos |
| {.dense}         |          |                                        |

Documented `gender` values are:

```text
0 = male
1 = female
2 = both
```

Addon tattoo entries appear in the Addon Tattoos list.

The custom tattoo assets themselves must already be streamed by another resource. vMenu does not create or stream the tattoo assets for you.

> `name` and `collectionName` must match the streamed overlay data. Incorrect hashes or names prevent the tattoo from displaying.
> {.is-warning}

Duplicate entries using the same collection and tattoo names are rejected.

Invalid `tattoos.json` errors are reported on the client side, so check the FiveM F8 console when debugging custom tattoo entries.

---

## Menu and Player Functionality

vMenu exposes a large collection of server-controlled menu functionality.

Access can vary according to ACE configuration.

Broad functional areas include:

### Player Management

Player-facing options can control supported character and gameplay settings.

Server owners can expose only the portions appropriate for their server by configuring the corresponding ACE permissions.

### Vehicle Management

vMenu includes vehicle-related menu functionality and can expose addon vehicle models configured through `addons.json`.

Vehicle extras can receive server-specific labels through `extras.json`.

### Character Customization

vMenu includes MP character customization functionality.

Custom streamed tattoos can be integrated through `tattoos.json`, while custom blendable face labels can be configured through `addons.json`.

### Weapons

Weapon-related menus can include base-game weapons and server-configured addon weapons.

Addon weapon components can also be registered in `addons.json`.

### World and Location Tools

Server-defined teleport destinations and blips can be loaded from `locations.json`.

### Administration

vMenu contains administrative functionality controlled through ACE permissions.

Sensitive functionality should only be granted to principals that require it.

> Never grant broad administrative ACE permissions to `builtin.everyone` unless every player is intentionally supposed to receive those capabilities.
> {.is-warning}

---

## Security and Permission Design

### Use Least Privilege

Build staff roles around the permissions they actually require.

For example:

```text
group.moderator
group.admin
group.owner
```

Avoid granting `.All` when a role only needs several specific functions.

### Separate Staff Levels

A useful permission design is:

```text
Normal Players
    ↓
Moderator
    ↓
Admin
    ↓
Owner
```

FiveM principal inheritance can reduce duplicate ACE entries, but the exact hierarchy is server-specific.

### Test With a Non-Staff Account

After changing permissions:

* [ ] Test the menu as a normal player
* [ ] Test each staff group
* [ ] Verify sensitive menus are hidden where expected
* [ ] Verify administrative actions are unavailable to unauthorized users
* [ ] Verify `builtin.everyone` does not contain unintended grants
* [ ] Restart the complete server after permission changes

---

## Troubleshooting {.tabset}

### Resource Does Not Load

Check the installation path.

Correct:

```text
resources/vMenu/fxmanifest.lua
```

Incorrect:

```text
resources/vMenu/vMenu/fxmanifest.lua
```

Also confirm the resource folder is exactly:

```text
vMenu
```

The folder name is case-sensitive.

### Permissions Do Not Update

A resource restart is not enough after editing `permissions.cfg`.

Restart the server so FXServer executes the permissions file again.

Also verify that `server.cfg` points to the file you actually edited.

### Menu Permissions Behave Unexpectedly

Check for broad `.All` permissions.

For example, if a principal receives:

```text
vMenu.PlayerOptions.All
```

individual grants or restrictions inside Player Options may not behave as expected.

Remove the broad `.All` grant when you need granular access.

### Configuration Does Not Load

Check:

* [ ] JSON syntax
* [ ] Missing commas
* [ ] Missing closing braces
* [ ] Missing closing brackets
* [ ] Duplicate entries
* [ ] Exact model names
* [ ] Correct configuration file
* [ ] Console errors

### Custom Tattoos Do Not Appear

Check:

* [ ] The tattoo resource streams correctly
* [ ] `collectionName` matches the streamed collection
* [ ] `name` matches the overlay name
* [ ] `gender` is `0`, `1`, or `2`
* [ ] `tattoos.json` contains valid JSON
* [ ] The client F8 console for vMenu errors

### Vehicle Extras Have Generic Names

Configure the vehicle in:

```text
extras.json
```

This only changes labels. The actual extra must exist on the vehicle model.

### Addon Content Does Not Appear

Check the relevant entry in:

```text
addons.json
```

Confirm that the spawn/model/component name exactly matches the content installed on the server.

---

## Compatibility

| Component                     | Status                |
| ----------------------------- | --------------------- |
| **FiveM**                     | Supported             |
| **FXServer**                  | Required              |
| **ACE permissions**           | Supported             |
| **Principals**                | Supported             |
| **MenuAPI**                   | Used by vMenu v2.1.0+ |
| **QBCore required**           | No                    |
| **Qbox required**             | No                    |
| **ESX required**              | No                    |
| **Standalone use**            | Supported             |
| **Addon vehicles**            | Configurable          |
| **Addon peds**                | Configurable          |
| **Addon weapons**             | Configurable          |
| **Addon weapon components**   | Configurable          |
| **Custom teleport locations** | Configurable          |
| **Custom blips**              | Configurable          |
| **Custom streamed tattoos**   | Configurable          |
| {.dense}                      |                       |

> Framework independence does not mean vMenu automatically integrates with framework jobs, permission groups, characters, garages, inventories, or other framework-specific systems.
> {.is-info}

---

## License

vMenu uses a custom license supplied in the official repository.

The license credits **Tom Grobbe** and permits use and modification with conditions.

Important restrictions documented by the project include:

* You must not claim the code as your own.
* Proper credit must be provided.
* vMenu or code taken from it may not be sold.
* A released modified version must link to the original repository or be distributed through a fork of the repository.

> Always review the current `LICENSE.md` in the official repository before redistributing or publishing modified vMenu code. The repository states that the license file takes precedence over license wording elsewhere in the project.
> {.is-warning}

---

## Project Status

The official documentation labels this project:

```text
vMenu (Legacy)
```

The creator states that the legacy project is no longer actively supported.

It may still receive:

* Small updates from merged community pull requests
* Updates related to new FiveM content

Development effort is directed toward vMenu Enhanced.

Support questions may still be discussed through the creator's community channels, but the documentation states that assistance for the legacy project is community-provided and not guaranteed.

---

## Official Links

* [Official GitHub Repository](https://github.com/TomGrobbe/vMenu)
* [Official GitHub Releases](https://github.com/TomGrobbe/vMenu/releases)
* [vMenu Legacy Documentation](https://docs.vespura.com/vmenu/legacy/)
* [Installation](https://docs.vespura.com/vmenu/legacy/installation/)
* [Configuration Options](https://docs.vespura.com/vmenu/legacy/configuration/)
* [Permissions Guide](https://docs.vespura.com/vmenu/legacy/permissions/)
* [Permissions Reference](https://docs.vespura.com/vmenu/legacy/permissions/permissions/)
* [Default permissions.cfg](https://docs.vespura.com/vmenu/legacy/permissions/default-permissions/)
* [addons.json](https://docs.vespura.com/vmenu/legacy/configuration/addons-json/)
* [extras.json](https://docs.vespura.com/vmenu/legacy/configuration/extras-json/)
* [locations.json](https://docs.vespura.com/vmenu/legacy/configuration/locations-json/)
* [model-whitelists.json](https://docs.vespura.com/vmenu/legacy/configuration/model-whitelists-json/)
* [tattoos.json](https://docs.vespura.com/vmenu/legacy/configuration/tattoos-json/)
* [Troubleshooting & Support](https://docs.vespura.com/vmenu/legacy/support/)
* [F.A.Q.](https://docs.vespura.com/vmenu/legacy/faq/)
* [License](https://github.com/TomGrobbe/vMenu/blob/master/LICENSE.md)

---

## Before You Install

* [ ] Confirm your FXServer artifacts are current
* [ ] Download vMenu only from the official repository
* [ ] Use a packaged GitHub release
* [ ] Name the resource folder exactly `vMenu`
* [ ] Confirm `fxmanifest.lua` is directly inside the resource folder
* [ ] Back up existing configuration before updating
* [ ] Configure `permissions.cfg`
* [ ] Execute `permissions.cfg` before `ensure vMenu`
* [ ] Review ACE grants assigned to `builtin.everyone`
* [ ] Avoid broad `.All` grants when granular permissions are required
* [ ] Validate edited JSON configuration files
* [ ] Restart the full server after changing permissions
* [ ] Test permissions with normal and staff accounts
* [ ] Review the project's legacy support status

---

## Credits

Created by **Tom Grobbe (Vespura)** with contributions from the vMenu project contributors.

vMenu uses **MenuAPI**, created for vMenu by Tom Grobbe. Earlier vMenu versions used a modified NativeUI implementation, with upstream work credited by the project to Guad, the CitizenFX Collectives, and Tom Grobbe.

SantosDB provides resource information and source references.

SantosDB does not provide support for vMenu and does not distribute the resource.

Resource rights belong to the project authors and rights holders.