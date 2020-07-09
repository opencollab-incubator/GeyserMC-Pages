---
layout: default
title: Config
parent: Geyser Connect
nav_order: 1
---
# Config
* `address` - The IP address that will listen for connections.
* `remote-address` - The IP address to forward players to, this needs to be accessible by the client. Set it to `auto` to grab your public IP automatically.
* `port` - The port that will listen for connections.
* `debug-mode` - If debug messages should be sent through console.
* `max-players` - Maximum amount of players that can connect.
* `motd` - MOTD to display.
* `geyser`
  * `port` - The port that will listen for connections.
  * `debug-mode` - If debug messages should be sent through the console, has to be enabled in both places to work.
  * `shutdown-time` - The time to wait after the last player disconnects to shutdown the proxy, in seconds. Set to -1 to disable.
* `servers` - A list of servers to show for everyone build from `address`, `port`, `online` and `bedrock` all optional apart from address.
* `custom-servers`
  * `enabled` - Should custom servers be enabled for users.
  * `max` - Max amount of custom servers per user.
  * `storage-type` - Storage engine for custom servers. Can be `json`, `sqlite`, `mysql`
  * `mysql` - Connection information for the MySQL database if enabled

The default config can be found [here](https://github.com/GeyserMC/GeyserConnect/blob/master/src/main/resources/config.yml).
