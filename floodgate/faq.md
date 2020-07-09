---
layout: default
title: FAQ
parent: Floodgate
nav_order: 3
---
# FAQ
## How do I add players to the whitelist when using Floodgate?
There are two ways you can do this. The first way is to turn off the whitelist using `/whitelist off`, then get the Geyser player to join, then run `/whitelist add "username"`, then turn the whitelist back on using `/whitelist on`. The second way is to add the player's UUID as given by Floodgate to the whitelist.json file and then run `/whitelist reload`.

## How do I find a player's UUID without them joining when using Floodgate?
First, you'll need to get the XUID of the player. There are several third-party websites to find this, for example [this one](https://cxkes.me/xbox/xuid) (unaffiliated with Geyser). Make sure to choose "
Hexidecimal". You'll need to enter the player's Xbox gamertag, and once submitted it should display the XUID in the format of `xxxxxxxxxxxxxxxx`. In order to turn the XUID into a UUID that Java Edition can recognize, you just need to put the XUID in this format: `00000000-0000-0000-xxxx-xxxxxxxxxxxx`. If formatted right, Java Edition should accept it as a UUID.
