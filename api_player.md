---
title: Player
parent: API v1
nav_order: 1
permalink: /api/v1/player
---

# Player

Returns player data for the requested player UUID or username. UUIDs must be in expanded format.

Endpoint: `/player/{uuid}` or `/player/{username}`

## Response
### `player_deaths`

| Key    | Type   | Description                                     |
|--------|--------|-------------------------------------------------|
| date   | string | Date in `Day, HH:MM:SS` format                 |
| weapon | string | Name of Weapon                                  |
| victim | string | Person Killed \(returns requested player name\) |
| killer | string | Killer \(returns who killed requested player\)  |

