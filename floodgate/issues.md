---
layout: default
title: Common Issues
parent: Floodgate
nav_order: 1
---
# Common Issues
## Skins
Due to how Minecraft: Java Edition handles skins, all Bedrock players will appear as Steve or Alex to other Java players. 

## Access token can not be null or empty
This may be because you forgot to set the auth-type in the config to `floodgate`. If that isn't it, check to make sure your config contains the line `floodgate-key-file: public-key.pem`. If not, just copy that in directly.

## Invalid packet id: 27
This usually means one of two things:

* You did not follow the Floodgate instructions properly. However, in an unlikely scenario, this could also be an error related to uploading through FTP. Using ascii will not work here, and you need to make sure you're on binary when uploading.
* You're trying to log in without an Xbox account. Floodgate requires an Xbox account to authenticate the Bedrock player.

## Whitelist command not working
See [this page](faq#how-do-i-add-players-to-the-whitelist-when-using-floodgate). 

### -- MOVE TO AN FAQ PAGE? --

## Obtaining UUIDs for Floodgate players
Check the server log for their UUIDs, or use [this method](faq#how-do-i-find-a-players-uuid-without-them-joining-when-using-floodgate).

### -- WILL BE MOVED TO GEYSER ADDONS --

## Using PlaceholderAPI
If you're using the Bukkit version of Floodgate, download the Placeholder plugin [here](https://github.com/rtm516/FloodgatePlaceholders/). Using the placeholders shouldn't require additional setup other than having [PlaceholderAPI](https://www.spigotmc.org/resources/6245/) installed. See the section above on installing Floodgate on backend servers if you wish to use this on BungeeCord.

## Using Skript
If you're using the Bukkit version of Floodgate, there is an unofficial plugin that adds Skript support [here](https://github.com/DoctorMacc/floodgate-skript).
