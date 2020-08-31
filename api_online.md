---
title: Online
parent: API v1
nav_order: 5
permalink: /api/v1/online
---

# Online (Server Stats)

Returns server statistics including TPS, sessions, play time, new/unique players, downtime, and averages of the data.

Endpoint: `/online/{server}`
<br />
Valid server names: `hub, anarchy`

## Response

### trends
### `new_players_30d_trend` `new_players_30d_avg_trend` `unique_players_30d_trend` `unique_players_30d_avg_trend` `sessions_30d_trend` `sessions_length_30d_trend` `playtime_30d_trend` `playtime_30d_avg_trend`

| Key       | Type    | Description                                                 |
|-----------|---------|-------------------------------------------------------------|
| text      | string  | Number or time associated with the trend                    |
| direction | string  | Returns "\+" or "\-" to declare direction of the trend      |
| reversed  | boolean | Whether or not the trend has reversed since the last period |
