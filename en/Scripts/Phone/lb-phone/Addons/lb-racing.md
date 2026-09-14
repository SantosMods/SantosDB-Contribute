---
title: lb-racing
description: Paid FiveM racing system with race creation, track creation, standalone tablet use, and LB Phone and LB Tablet integration.
published: true
date: 2026-09-14T01:53:18.326Z
tags: script, ui, vehicles, racing
editor: markdown
dateCreated: 2026-09-14T01:53:18.326Z
---

# lb-racing [![](https://badges.5metrics.dev/lb-racing/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/lb-racing)

Paid FiveM racing system with race creation, track creation, standalone tablet use, and LB Phone and LB Tablet integration.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field        | Information |
| ------------ | ----------- |
| **Name**     | `lb-racing` |
| **Creator**  | LB Scripts  |
| **Type**     | Script      |
| **Category** | Racing      |
| **Game**     | FiveM       |
| **Price**    | Paid        |
| **License**  | Unknown     |
| {.dense}     |             |

---

## Resource Details {.tabset}

### Overview

`lb-racing` is a FiveM racing system with race and track creation.

It can run through LB Phone, LB Tablet, or its standalone racing tablet.

### Requirements

The official documentation requires:

* `oxmysql`
* MariaDB 10.11 or newer
* Up-to-date FiveM server artifacts
* OneSync Infinity

### Database

With MariaDB 10.11 or newer, the resource can add its required SQL tables automatically.

The package also includes:

```text
racing.sql
default-tracks.sql
```

`default-tracks.sql` can be used to install the supplied default tracks.

---

## Installation

### Installation Checklist

* [ ] Install MariaDB 10.11 or newer
* [ ] Install `oxmysql`
* [ ] Enable OneSync Infinity
* [ ] Download `lb-racing` from the authorized source
* [ ] Configure database setup
* [ ] Import default tracks if desired
* [ ] Configure the racing system
* [ ] Add `lb-racing` to `server.cfg`
* [ ] Test race and track creation

### Resource Order

```cfg
start oxmysql
start lb-racing
```

---

## Configuration

The main configuration file is:

```text
lb-racing/config/config.lua
```

Track creator props are configured in:

```text
lb-racing/config/props.lua
```

The framework integration can use:

```lua
Config.Framework = "auto"
```

The standalone racing tablet is configured through `Config.Standalone`.

LB Phone and LB Tablet app behavior is configured through `Config.App`.

---

## Usage

The standalone configuration supports a command named:

```text
racingtablet
```

The documented default bind is:

```text
F4
```

These values can be changed in configuration.

---

## Links

* [Official Documentation](https://docs.lbscripts.com/racing/)
* [Installation](https://docs.lbscripts.com/racing/installation/)
* [Configuration](https://docs.lbscripts.com/racing/configuration/)
* [Authorized Store](https://store.lbscripts.com/)

---

## Credits

Created and maintained by **LB Scripts**.

SantosDB provides resource information and source references.

Resource rights belong to LB Scripts and other applicable rights holders.
