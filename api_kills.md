---
title: Kills
parent: API v1
nav_order: 4
permalink: /api/v1/kills
---

# Kills

Returns cumulative player and mob deaths for the requested server.

Endpoint: `/kills/{server}`
<br />
Valid server names: `hub, anarchy`

# Response

## "numbers"

| Key                   | Type   | Description                        |
|-----------------------|--------|------------------------------------|
| player\_kdr\_avg      | number | All\-time player KDR               |
| player\_kdr\_avg\_7d  | number | Player KDR over the past 7 days    |
| player\_kdr\_avg\_30d | number | Player KDR over the past 30 days   |
| player\_kills\_total  | number | All\-time player kills             |
| player\_kills\_7d     | number | Kills over the past 7 days         |
| player\_kills\_30d    | number | Kills over the past 30 days        |
| deaths\_7d            | number | Total deaths over the past 7 days  |
| deaths\_30d           | number | Total deaths over the past 30 days |
| deaths\_total         | number | All\-time deaths                   |
| mob\_deaths\_7d       | number | Mob deaths over the past 7 days    |
| mob\_deaths\_30d      | number | Mob deaths over the past 30 days   |
| mob\_deaths\_total    | number | All\-time mob deaths               |
| mob\_kills\_7d        | number | Mob kills over the past 7 days     |
| mob\_kills\_30d       | number | Mob kills over the past 30 days    |
| mob\_kills\_total     | number | All\-time mob kills                |
| mob\_kdr\_7d          | number | Mob KDR over the past 7 days       |
| mob\_kdr\_30d         | number | Mob KDR over the past 30 days      |
| mob\_kdr\_total       | number | All\-time mob KDR                  |

