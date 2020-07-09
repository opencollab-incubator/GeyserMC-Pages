---
layout: default
title: Setup
parent: Geyser Connect
nav_order: 0
---
# Setup

## Installation
(For GeyserConnect to work you need 2 UDP ports open, by default these are `19132` and `19133`.)
1. Download the latest build from [Jenkins](https://ci.nukkitx.com/job/GeyserMC/job/GeyserConnect/job/master/)
2. Edit the config as needed
3. Start the server as you do with a normal Geyser install. EG: `java -Xms1024M -jar GeyserConnect.jar` (More info on [Creating a Startup Script](Creating-a-Startup-Script))
4. Connect to it to make sure its all working.

## DNS and Docker
There are both [DNS](https://github.com/GeyserMC/GeyserConnect/tree/master/bind9) (using bind9) and [Docker](https://github.com/GeyserMC/GeyserConnect/tree/master/docker) configs in the repo if you would like to use them.