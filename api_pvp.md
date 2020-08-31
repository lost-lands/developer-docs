---
title: PVP
parent: API v1
nav_order: 2
permalink: /api/v1/pvp
---

# PVP

Returns the last 100 PVP kills on the requested server.

Endpoint: `/pvp/{server}`
<br />
Valid server names: `hub, anarchy`

## Response

### `player_kills`

| Key    | Type   | Description                      |
|--------|--------|----------------------------------|
| date   | string | Time in `Day, HH:MM:SS` format   |
| weapon | string | Name of weapon used              |
| victim | string | Username of player killed        |
| killer | string | Username of killer               |


