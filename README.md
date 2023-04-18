# Cruelty Squad: Apocrypha Mode

Apocrypha Mode is an overhaul patch for Cruelty Squad that adds a base set of mod/custom-content related functionality for both players and modders. 

## Install

_Reminder: You must own a copy of the game for the installer/patcher to work._

Installer downloads are made available in the [Releases section](https://github.com/disco0/apocrypha-mode/releases/latest) of this repository. As of writing, the current intent is to release """stable""" builds of Apocrypha here, with more frequent test builds available in the #modifications discord channel.

The installer/patcher godot project is also available separately [here](https://github.com/disco0/apocrypha-patcher)

## Features

In addition to expanding on CruS Mod Base and CruS Modloader—newer versions of which are Apocrypha Mode's base—other changes have been made at lower levels, including:

**Custom Godot 3.5 build**

- Can now take advantage of newer engine features added since release, such as in-game navigation mesh generation and occluder nodes. 

- Beyond engine updates, support for building asset import artifacts in game has been patched in, allowing for modders/mappers to completely avoid having to generate and manage `.import` files in most cases.
 
**Zip archive support**

- Added via gdnative library for drag and drop [content installer](https://gist.github.com/disco0/090aa50673122c4731552a1df1e5998a#addon-content-installer). Native engine support will _hopefully_ be backported to `3.x`, [eventually](https://github.com/godotengine/godot/pull/65281).

**Modding API**

- The `Mod` singleton has been expanded with new signals, and utility functions to make hooking into common game logic simpler, or add new functionality like creating custom commands, etc.

- Very much work in progress, however the working API interface documented [here](https://gist.github.com/disco0/090aa50673122c4731552a1df1e5998a#file-01-api-md) is effectively stable.


## ~~Building~~ (WIP)

Apocrypha is a heavily rewritten version the game based on decompilation artifacts. The project will be pushed to this repository when cloning the project repo is no longer effectively be pirating the game (similar to the installer).

In the meantime, full project backups are available in the #modifications channel as well as other necessary items, e.g. custom godot build templates for those interested.
