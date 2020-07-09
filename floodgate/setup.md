---
layout: default
title: Setup
parent: Floodgate
nav_order: 0
---
# Setup
## Setting Up
**NOTE: Floodgate does not replace the Geyser jar. If you are running a plugin version of Geyser, you still MUST have Geyser installed.**

*Any reference to Spigot here also refers to compatible server softwares such as Paper.*

### Plugin Setup (You have Geyser and Floodgate on the same server)

For multi-server setups: you only are required to install Floodgate on the BungeeCord or Velocity instance unless you want to use the Floodgate API on the other servers - see below for the installation process.

*If using Velocity*: Set `player-info-forwarding-mode` to `LEGACY` in `velocity.toml` 

- Download the Floodgate plugin from [here](https://ci.nukkitx.com/job/GeyserMC/job/Floodgate/job/development/) and add it to your plugins folder.
- Change the `auth-type` in the Geyser config to `floodgate`.
- Restart/start up the server.

### Standalone Setup (Geyser and Floodgate are in separate places)

- Download the Floodgate plugin from [here](https://ci.nukkitx.com/job/GeyserMC/job/Floodgate/job/development/) and add it to your plugins folder.
- Run the server with Floodgate.
- *Copy* the `public-key.pem` file in the Floodgate config folder to the same directory as Geyser (standalone) or Geyser's config folder (plugin versions). **DO NOT DISTRIBUTE THIS KEY TO ANYBODY!** This key is what allows for Bedrock accounts to bypass the Java Edition authentication, and if anyone gets ahold of this, they can wreak havoc on your server.
- Change the `auth-type` in the Geyser config to `floodgate`.

### Running Floodgate on Spigot servers behind BungeeCord or Velocity

This is only needed when you want to use the Floodgate API on your Spigot server(s).

- Download the Floodgate plugin from [here](https://ci.nukkitx.com/job/GeyserMC/job/Floodgate/job/development/) and install it as a plugin on both BungeeCord/Velocity and the Spigot server(s).
- Enable `ip_forwarding` in your BungeeCord `config.yml` if using BungeeCord
- Set `player-info-forwarding-mode` to `LEGACY` in `velocity.toml` if using Velocity
- Set `bungeecord` to `true` in your `spigot.yml`
- Start the proxy server.
- Edit the Floodgate config on your proxy server and set `send-floodgate-data` to `true`.
- *Copy* both key files in the Floodgate config folder to Spigot Floodgate's config folder. **DO NOT DISTRIBUTE THIS KEY TO ANYBODY!** This key is what allows for Bedrock accounts to bypass the Java Edition authentication, and if anyone gets ahold of this, they can wreak havoc on your server.
- Restart the Spigot servers and proxy server.
