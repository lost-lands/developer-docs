---
title: Performance
parent: API v1
nav_order: 3
permalink: /api/v1/performance
---

# Performance

Returns server performance for the select server

#### HTTP
`/performance/{server}`
#### Valid Servers
Valid server names: `anarchy` `crystalpvp`

#### NodeJS / JavaScript
```javascript
const server = "anarchy";
v1.performance(server, function(err, data) {
    if (err) {
        console.error(err);
    } else {
        //data is an array of all documented performance data for the requested server
        console.log(data);
    }
});
```

## Response

### `insights`

| Key                | Type   | Description                         |
|--------------------|--------|-------------------------------------|
| low\_tps\_players  | string | Players online during last TPS drop |
| low\_tps\_chunks   | string | Chunks loaded during last TPS drop  |
| low\_tps\_entities | string | Total entities during last TPS drop |

### `numbers`

| Key                   | Type   | Description                          |
|-----------------------|--------|--------------------------------------|
| tps\_24h              | number | Average TPS over 24 hours            |
| tps\_7d               | number | Average TPS over 7 days              |
| tps\_30d              | number | Average TPS over 30 days             |
| low\_tps\_spikes\_24h | number | Average low TPS spikes over 24 hours |
| low\_tps\_spikes\_7d  | number | Average low TPS spikes over 7 days   |
| low\_tps\_spikes\_30d | number | Average low TPS spikes over 30 days  |
| entities\_24h         | number | Average entities over 24 hours       |
| entities\_7d          | number | Average entities over 7 days         |
| entities\_30d         | number | Average entities over 30 days        |
| chunks\_24h           | number | Average loaded chunks over 24 hours  |
| chunks\_7d            | number | Average loaded chunks over 7 days    |
| chunks\_30d           | number | Average loaded chunks over 30 days   |
| server\_downtime\_24h | string | Total server downtime over 24 hours  |
| server\_downtime\_7d  | string | Total server downtime over 7 days    |
| server\_downtime\_30d | string | Total server downtime over 30 days   |




