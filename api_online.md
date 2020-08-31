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

| Key                                | Type   | Description                                                                             |
|------------------------------------|--------|-----------------------------------------------------------------------------------------|
| average\_tps                       | number | All\-time average TPS                                                                   |
| downtime                           | string | Total downtime                                                                          |
| low\_tps\_spikes                   | number | Total low TPS spikes                                                                    |
| new\_players\_24h                  | number | Total new players over the past 24 hours                                                |
| new\_players\_24h\_avg             | number | Average new players over the past 24 hours                                              |
| new\_players\_30d                  | number | Total new players over the past 30 days                                                 |
| new\_players\_30d\_avg             | number | Average new players over the past 30 days                                               |
| new\_players\_30d\_avg\_trend      | Array  | see "trends"                                                                            |
| new\_players\_30d\_trend           | Array  | see "trends"                                                                            |
| new\_players\_7d                   | number | Total new players over the past 7 days                                                  |
| new\_players\_7d\_avg              | number | Average new players within 7 days                                                       |
| new\_players\_retention\_24h       | number | Total players who have stayed within the past 24 hours                                  |
| new\_players\_retention\_24h\_perc | string | Percentage of new players who have stayed versus all new players over the past 24 hours |
| new\_players\_retention\_30d       | number | Total players who have stayed within the past 30 days                                   |
| new\_players\_retention\_30d\_perc | string | Percentage of new players who have stayed versus all new players over the past 30 days  |
| new\_players\_retention\_7d        | number | Total players who have stayed within the past 7 days                                    |
| new\_players\_retention\_7d\_perc  | string | Percentage of new players who have stayed versus all new players over the past 7 days   |
| playtime\_24h                      | string | Total playtime over the past 24 hours                                                   |
| playtime\_24h\_avg                 | string | Average playtime over the past 24 hours                                                 |
| playtime\_30d                      | string | Total playtime over the past 30 days                                                    |
| playtime\_30d\_avg                 | string | Average playtime over the past 30 days                                                  |
| playtime\_30d\_avg\_trend          | Array  | see "trends"                                                                            |
| playtime\_30d\_trend               | Array  | see "trends"                                                                            |
| playtime\_7d                       | string | Total playtime over the past 7 days                                                     |
| playtime\_7d\_avg                  | string | Average playtime over the past 7 days                                                   |
| session\_length\_24h\_avg          | string | Average session length over the past 24 hours                                           |
| session\_length\_30d\_avg          | string | Average session length over the past 30 days                                            |
| session\_length\_30d\_trend        | Array  | see "trends"                                                                            |
| session\_length\_7d\_avg           | string | Average session length over the past 7 days                                             |
| sessions\_24h                      | number | Number of sessions over the past 24 hours                                               |
| sessions\_30d                      | number | Number of sessions over the past 30 days                                                |
| sessions\_30d\_trend               | Array  | see "trends"                                                                            |
| sessions\_7d                       | number | Number of sessions over the past 7 days                                                 |
| unique\_players\_24h               | number | Total unique players over the past 24 hours                                             |
| unique\_players\_24h\_avg          | Array  | see "trends"                                                                            |
| unique\_players\_30d               | number | Total unique players over the past 30 days                                              |
| unique\_players\_30d\_avg          | number | Average unique players over the past 30 days                                            |
| unique\_players\_30d\_avg\_trend   | Array  | see "trends"                                                                            |
| unique\_players\_30d\_trend        | Array  | see "trends"                                                                            |
| unique\_players\_7d                | number | Total unique players over the past 7 days                                               |
| unique\_players\_7d\_avg           | number | Average unique players over the past 7 days                                             |


### trends
### `new_players_30d_trend` `new_players_30d_avg_trend` `unique_players_30d_trend` `unique_players_30d_avg_trend` `sessions_30d_trend` `sessions_length_30d_trend` `playtime_30d_trend` `playtime_30d_avg_trend`
{: .lh-default }

| Key       | Type    | Description                                                 |
|-----------|---------|-------------------------------------------------------------|
| text      | string  | Number or time associated with the trend                    |
| direction | string  | Returns "\+" or "\-" to declare direction of the trend      |
| reversed  | boolean | Whether or not the trend has reversed since the last period |
