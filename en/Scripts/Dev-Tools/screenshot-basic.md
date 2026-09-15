---
title: screenshot-basic
description: CitizenFX FiveM resource for capturing client game render targets as screenshots through exports.
published: true
date: 2026-09-14T01:42:13.699Z
tags: developer-tool, script, standalone, screenshots
editor: markdown
dateCreated: 2026-09-14T01:42:13.699Z
---

# screenshot-basic [![](https://badges.5metrics.dev/screenshot-basic/servers.svg?style=for-the-badge)](https://5metrics.dev/resource/screenshot-basic)

CitizenFX FiveM resource for capturing client game render targets as screenshots through exports.

> SantosDB links to the source project. SantosDB does not own, maintain, or distribute this resource.
> {.is-info}

---

## Resource Information

| Field         | Information        |
| ------------- | ------------------ |
| **Name**      | `screenshot-basic` |
| **Creator**   | CitizenFX          |
| **Type**      | Script             |
| **Category**  | Screenshot Utility |
| **Game**      | FiveM              |
| **Price**     | Free               |
| **License**   | MIT                |
| **Framework** | Standalone         |
| {.dense}      |                    |

---

## Resource Details {.tabset}

### Overview

`screenshot-basic` captures a client's game render target using FiveM.

The resource exposes screenshot functionality through exports rather than directly usable commands.

### Client API

Documented client exports include:

```text
requestScreenshot
requestScreenshotUpload
```

`requestScreenshot` returns a screenshot as a data URI.

`requestScreenshotUpload` captures a screenshot and uploads it to a remote HTTP endpoint using `multipart/form-data`.

Supported image encodings include:

```text
png
jpg
webp
```

### Server API

The server API provides:

```text
requestClientScreenshot
```

This requests a screenshot from a specified client.

The official documentation states that the server API requires at least FiveM client version `1129160` and server pipeline `1011`.

---

## Installation

### Installation Checklist

* [ ] Update `cfx-server-data`
* [ ] Download `screenshot-basic`
* [ ] Place `screenshot-basic` in your resources folder
* [ ] Add it to your startup configuration
* [ ] Start the resource
* [ ] Test the required export from your dependent resource

### Resource Order

```cfg
ensure screenshot-basic
```

Start it before resources that require its exports.

---

## Usage

Example client screenshot:

```lua
exports['screenshot-basic']:requestScreenshot(function(data)
    print(data)
end)
```

> The returned screenshot can contain substantial image data. The official documentation warns against sending the `requestScreenshot` data URI through server events.
> {.is-warning}

---

## Compatibility

| Item                             | Information        |
| -------------------------------- | ------------------ |
| **Game**                         | FiveM              |
| **Framework**                    | Standalone         |
| **Client screenshots**           | Supported          |
| **Screenshot uploads**           | Supported          |
| **Server-requested screenshots** | Supported          |
| **Resource name**                | `screenshot-basic` |
| {.dense}                         |                    |

---

## Links

* [Official GitHub Repository](https://github.com/citizenfx/screenshot-basic)

---

## Before You Install

* [ ] Update `cfx-server-data`
* [ ] Confirm dependent resources use supported exports
* [ ] Verify remote upload endpoints before using uploads
* [ ] Do not expose private upload credentials
* [ ] Check client and server build requirements for server-requested screenshots

---

## Credits

Created and maintained by **CitizenFX** and project contributors.

SantosDB provides resource information and source references.

Resource rights belong to the project authors and rights holders.
