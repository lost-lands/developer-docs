---
title: Performance
parent: API v1
nav_order: 3
permalink: /api/v1/performance
---

# Performance

Returns server performance for the select server

Endpoint: `/performance/{server}`
<br />
Valid server names: `hub, anarchy`

## Response

### "numbers"
| Key         | Value                                 |
|-------------|---------------------------------------|
| tps_7d      | Average TPS over the last 7 days      |
| entities_7d | Average entities over the last 7 days |
|             |                                       |

