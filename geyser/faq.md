---
layout: default
title: FAQ
parent: Geyser
nav_order: 5
---
# FAQ
## How Does it Work?
Geyser works as a translator, translating both the incoming and outgoing packets to a format both the client and server can understand. With this being said, it emulates a Minecraft: Java Edition client, so the server actually thinks you're joining from Java Edition. Regardless of the server or what plugins it has installed, you can join it with Geyser (as long as the server supports the latest Minecraft version).

## What plugins don't work with Geyser?
* [JPremium](https://www.spigotmc.org/resources/27766/) alters the UUID of a player causing Floodgate to not be able to get the Bedrock data from its map.
* [ProtocolSupport](https://www.spigotmc.org/resources/7201/) sometimes causes issues with Floodgate saying `Invalid packet id: 27`. Use [ViaVersion](https://www.spigotmc.org/resources/19254/) instead if this keeps occurring.
* [TCPShield](https://tcpshield.com/) causes Floodgate not to be able to authenticate.

If you come across any more please let us know via [Discord](http://discord.geysermc.org).

## Which plugin version of Geyser do I need?
This is a non-complete list of what platform each plugin version of Geyser is for, the standalone version can be used for any as it isn't a plugin.
* Geyser-Spigot works with:
  * [Spigot](https://www.spigotmc.org/)
  * [Paper](https://papermc.io/downloads) (recommended)
  * Any other forks of the above
* Geyser-Bungee works with:
  * [BungeeCord](https://www.spigotmc.org/wiki/bungeecord/)
  * [Waterfall](https://papermc.io/downloads#Waterfall)
  * Any other forks of the above
* Geyser-Velocity works with [Velocity](https://www.velocitypowered.com/)
* Geyser-Sponge works with [SpongeVanilla or SpongeForge](https://www.spongepowered.org/)

## If using BungeeCord or another fork, where do I need to put Geyser/Floodgate?
You only need Geyser and/or Floodgate on the BungeeCord server.

## Can I use Geyser with Pterodactyl Panel?
Yes, we have an official egg for the standalone version, it supports auto-updating and has all config options easily editable. You can find it [here](https://github.com/GeyserMC/pterodactyl-stuff), just download the JSON egg and import it into your panel.

## Can I use Geyser with Ngrok?
Unfortunately Ngrok is TCP-only, so you will not be able to use Geyser with Ngrok.

## Can I use Buycraft with Geyser?
You sure can! Buycraft supports Java & Bedrock players via the Offline store mode **(Recommended to be used with Floodgate)**
### Steps to create a store to support both versions
- Buycraft-> Create Webstore
- Select Game-> Minecraft Offline
- Continue-> Click "Create my Webstore"
- Name your server & Select currency-> Continue
- Select Game Server-> Continue
- Download the plugin version that best suits your server.
- Execute the secret command from your servers console

Your store is now setup to support Bedrock & Java players

**(PLEASE NOTE, BEDROCK PLAYERS MUST INCLUDE THE PREFIX)**

## What languages does Geyser support?
We aim to support any of the bedrock languages, see [here](https://translate.geysermc.org/) for our Crowdin page and below is a list of all the language codes.
|Name                        |Code |
|----------------------------|-----|
|Bulgarian                   |bg_bg|
|Czech                       |cs_cz|
|Danish                      |da_dk|
|German                      |de_de|
|Greek                       |el_gr|
|British English             |en_gb|
|American English            |en_us|
|Spanish                     |es_es|
|Mexican Spanish             |es_mx|
|Finnish                     |fi_fi|
|Canadian French             |fr_ca|
|French                      |fr_fr|
|Hungarian                   |hu_hu|
|Indonesian                  |id_id|
|Italian                     |it_it|
|Japanese                    |ja_jp|
|Korean                      |ko_kr|
|Dutch                       |nl_nl|
|Norwegian Bokmål            |nb_no|
|Polish                      |pl_pl|
|Brazilian Portuguese        |pt_br|
|Portuguese                  |pt_pt|
|Russian                     |ru_ru|
|Slovak                      |sk_sk|
|Swedish                     |sv_se|
|Turkish                     |tr_tr|
|Ukrainian                   |uk_ua|
|Chinese Simplified (China)  |zh_cn|
|Chinese Traditional (Taiwan)|zh_tw|
