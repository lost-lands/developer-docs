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
| date   | string | Date in  `Day, HH:MM:SS` format                 |
| weapon | string | Name of Weapon                                  |
| victim | string | Person Killed \(returns requested player name\) |
| killer | string | Killer \(returns who killed requested player\)  |

### `player_kills`

| Key    | Type   | Description                                           |
|--------|--------|-------------------------------------------------------|
| date   | string | Date in  `Day, HH:MM:SS` format                       |
| weapon | string | Name of Weapon                                        |
| victim | string | Person Killed \(returns who killed requested player\) |
| killer | string | Killer \(returns requested player name\)              |

### `online_activity`

| Key                           | Type   | Description                                  |
|-------------------------------|--------|----------------------------------------------|
| session\_count\_7d            | number | Number of sessions over the past 7 days      |
| session\_count\_30d           | number | Number of sessions over the past 30 days     |
| average\_session\_length\_7d  | string | Average session length over the past 7 days  |
| average\_session\_length\_30d | string | Average session length over the past 30 days |
| median\_session\_length\_7d   | string | Median session length over the past 7 days   |
| median\_session\_length\_7d   | string | Median session length over the past 30 days  |
| playtime\_7d                  | string | Total Playtime over the past 7 days          |
| playtime\_30d                 | string | Total Playtime over the past 30 days         |
| active\_playtime\_7d          | string | Active playtime over the past 7 days         |
| active\_playtime\_30d         | string | Active playtime over the past 30 days        |
| afk\_time\_7d                 | string | AFK time over the past 7 days                |
| afk\_time\_30d                | string | AFK time over the past 30 days               |
| player\_kill\_count\_7d       | number | Number of PVP kills over the past 7 days     |
| player\_kill\_count\_30d      | number | Number of PVP kills over the past 30 days    |
| mob\_kill\_count\_7d          | number | Number of mob kills over the past 7 days     |
| mob\_kill\_count\_30d         | number | Number of mob kills over the past 30 days    |
| death\_count\_7d              | number | Total deaths over the past 7 days            |
| death\_count\_30d             | number | Total deaths over the past 30 days           |

### `info`

| Key                      | Type    | Description                               |
|--------------------------|---------|-------------------------------------------|
| banned                   | boolean | Whether or not the user is banned         |
| kick\_count              | number  | Total kicks (Includes AFK kick)         |
| last\_seen               | string  | Last seen in `Day, HH:MM:SS` format      |
| favorite\_server         | string  | Server the player spends the most time on |
| registered               | string  | First seen in `Day, HH:MM:SS` format     |
| average\_ping            | string  | Average ping                              |
| best\_ping               | string  | Best ping                                 |
| worst\_ping              | string  | Worst Ping                                |
| activity\_index          | string  | Calculated activity index                 |
| activity\_index\_group   | string  | Group calculated based on activity index  |
| session\_count           | number  | Total number of sessions                  |
| session\_median          | string  | Median number of sessions                 |
| longest\_session\_length | string  | Longest recorded session                  |
| playtime                 | string  | Total playtime                            |
| afk\_time                | string  | Total AFK time                            |
| active\_playtime         | string  | Total active playtime                     |
| player\_kill\_count      | string  | Total PVP kills                           |
| mob\_kill\_count         | string  | Total mob kills                           |


