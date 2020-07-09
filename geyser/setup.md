---
layout: default
title: Setup
parent: Geyser
has_children: true
nav_order: 0
---
# Setup
Bedrock clients will join through Geyser and it will handle all the packet translations. There are four different versions of Geyser: Geyser for Bukkit (works on derivatives such as Spigot and Paper), Geyser for BungeeCord (also works on Waterfall), Geyser for Velocity, and Geyser Standalone. The first three versions run as plugins and can be installed directly onto the server. The standalone version can be used in a similar way, except you run it separately. 

If you are running a server, it is highly recommended you use one of the plugin versions, and if you want to join a server that does not have Geyser installed, you can run the standalone version. If you use Pterodactyl Panel we have an egg for the standalone version, please see [here](faq#can-i-use-geyser-with-pterodactyl-panel) for more information.

If you're still having problems with Geyser not working or giving you an "Unable to connect to world" error, see the [Common Issues](issues) page.\
For more information, take a look at the [Understanding the Config](config) page, and the [FAQ](faq) page.\
And if you still have questions, feel free to join the [Discord](https://discord.geysermc.org) if you haven't already.

## Plugin Setup
1. Download a jar of Geyser from the [build server](https://ci.nukkitx.com/job/Geyser/job/master/) depending on what platform your server runs on.
2. Put Geyser in your plugins folder and start up the server.
3. Configure any needed options in the Geyser config. A description of all options of the config can be found on the [Understanding the Config](config) page. In most scenarios, this file should not need to be touched unless you intend to use [Floodgate]({{ site.baseurl }}/floodgate), or you're running your Java on a port that is not 25565. This may be the case if you are using a server hosting provider. Information on your hosting provider might be available on the [Supported Hosting Providers](providers) page. *You should not need to configure your remote address as the plugin handles this for you.*
4. Restart your server if needed.

Once you're done, open up Minecraft: Bedrock Edition and in the **Friends** tab, Geyser should show up there. If it does not show up, just add your IPv4 as an external server.

## Standalone Setup
Please keep in mind, you need some sort of computer or host to run Geyser Standalone on. Applications such as Termux on Android are capable of running Geyser, but this largely depends on how powerful your Android device is. Please do so at your own risk. Instructions to run Geyser on Termux can be found [here](#termux-android).

1. Download a jar of Geyser from the [build server](https://ci.nukkitx.com/job/Geyser/job/master/).
2. Create a new folder for Geyser, and drop the jar in there.
3. Create a new bat or startup script, similar to the one you'd use for a Bukkit server, and take a look at [this](startup) page for what to put into it.
4. Run the startup script/bat, and all the necessary files for Geyser will be created.

Once you're done, open up Minecraft: Bedrock Edition and in the **Friends** tab, Geyser should show up there. If it does not show up, just add your IPv4 as an external server.

## Termux (Android)
Please read the disclaimer [here](#standalone-setup) before continuing.
1. Download Termux
2. Follow [this guide](https://wiki.termux.com/wiki/Ubuntu)
3. Run `apt install default-jre`
4. Run `wget https://ci.nukkitx.com/job/GeyserMC/job/Geyser/job/master/lastSuccessfulBuild/artifact/bootstrap/standalone/target/Geyser.jar`
5. Run `java -jar Geyser.jar`

OR

We have an automated setup script for clean Termux installs, might not work for all users. If the manual guide above does not work, try this.
Run this to start the download/install:
```
curl https://gist.githubusercontent.com/rtm516/e3e07d6595ee41e05a38b03c0f4d7a80/raw/install.sh | bash
```
