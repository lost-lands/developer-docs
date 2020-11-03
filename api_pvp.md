---
title: PVP
parent: API v1
nav_order: 2
permalink: /api/v1/pvp
---

# PVP

Returns the last 100 PVP kills on the requested server.

#### HTTP
`/pvp/{server}`
#### Valid Servers
Valid server names: `anarchy` `crystalpvp`

#### NodeJS / JavaScript
```javascript
const server = "anarchy";
v1.pvp(server, function(err, kills) {
    if (err) {
        console.error(err);
    } else {
        //kills is an array of all documented player_kills data
        console.log(kills);
    }
});
```

## Response

### `player_kills`

| Key    | Type   | Description                      |
|--------|--------|----------------------------------|
| date   | string | Time in `Day, HH:MM:SS` format   |
| weapon | string | Name of weapon used              |
| victim | string | Username of player killed        |
| killer | string | Username of killer               |


