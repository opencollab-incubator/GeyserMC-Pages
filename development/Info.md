---
layout: default
title: Info
parent: Development
---
# Info
## Compiling
1. Clone the repo to your computer (EG: `git clone https://github.com/GeyserMC/Geyser.git`)
2. [Install Maven](https://maven.apache.org/install.html)
3. Navigate to the Geyser root directory and run `git submodule update --init --recursive`. This downloads all the needed submodules for Geyser and is a crucial step in this process.
4. Run `mvn clean install` and locate to the `bootstrap`, then your desired Geyser version, then `target` folder.

## Project layout
* `bootstrap` is where we hold the specific platform code. So if you're porting Geyser to a new platform, you likely want to be in here.
* `common` is where some data types are and other parts used in other plugins such as Floodgate.
* `connector` is where connections are handled and the data conversion is done. If adding in some new packet conversions you likely want to be in here.