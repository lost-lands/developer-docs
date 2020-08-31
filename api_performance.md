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

| Key      | Example Value | Description               |
|----------|---------------|---------------------------|
| tps\_24h | 20\.00        | Average TPS over 24 hours |
| tps\_7d  | 20\.00        | Average TPS over 7 days   |
| tps\_30d | 20\.00        | Average TPS over 30d      |



