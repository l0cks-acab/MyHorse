# MyHorse

**Author:** locks

## Overview

The **MyHorse** plugin for Rust allows players with the appropriate permissions to spawn, retrieve, and remove a custom horse. The plugin provides configurable cooldown times and messages, ensuring a personalized experience for each server.

## Features

- **Spawn a Custom Horse:** Players with the `myhorse.use` permission can spawn a horse directly in front of them.
- **Retrieve the Horse:** Players can move the horse back in front of them using the `/gethorse` command.
- **Remove the Horse:** Players can remove the horse using the `/removehorse` command.
- **Cooldown System:** A configurable cooldown timer prevents spamming the commands.
- **Building Block Check:** Players can't use the commands while building blocked.
- **Customizable Messages:** Server owners can change messages and cooldown timers via the configuration file.
- **Override Permission:** The `myhorse.override` permission removes the cooldown for specified players.

## Installation

1. **Download the Plugin:**
   - Download the `MyHorse.cs` plugin file.

2. **Place the Plugin:**
   - Place the `MyHorse.cs` file in your `oxide/plugins` directory.

3. **Reload Plugins:**
   - Use the command `oxide.reload MyHorse` to load the plugin.

## Configuration

The configuration file `MyHorse.json` is located in the `oxide/config` directory. Here are the available settings:

```json
{
  "CooldownTime": 300.0,
  "NoPermissionMessage": "You do not have permission to use this command.",
  "BuildingBlockedMessage": "You cannot use this command while building blocked.",
  "CooldownMessage": "You must wait {0} seconds before using this command again.",
  "HorseExistsMessage": "You already have a horse. Use /gethorse to retrieve it or /removehorse to remove it.",
  "HorseCreatedMessage": "Your horse has arrived!",
  "NoHorseToRetrieveMessage": "You do not have a horse to retrieve.",
  "MountedMessage": "You cannot use this command while mounted.",
  "OtherPlayerMountedMessage": "Someone is mounted on your horse. You cannot retrieve it right now.",
  "HorseMovedMessage": "Your horse has been moved in front of you.",
  "HorseRemovedMessage": "Your horse has been removed."
}
```

## Commands
/myhorse - `Spawns a custom horse in front of the player.`

/gethorse - `Moves the horse back in front of the player.`

/removehorse - `Removes the horse.`

## Permissions

myhorse.use - `Allows players to use the /myhorse, /gethorse, and /removehorse commands.`

myhorse.override - `Removes the cooldown for the player.`

## Installation

1. **Download the Plugin:**
   - Download the `MyHorse.cs` plugin file.

2. **Place the Plugin:**
   - Place the `MyHorse.cs` file in your `oxide/plugins` directory.

3. **Reload Plugins:**
   - Use the command `oxide.reload MyHorse` to load the plugin.

## Configuration

The configuration file `MyHorse.json` is located in the `oxide/config` directory. Here are the available settings:

```json
{
  "CooldownTime": 300.0,
  "NoPermissionMessage": "You do not have permission to use this command.",
  "BuildingBlockedMessage": "You cannot use this command while building blocked.",
  "CooldownMessage": "You must wait {0} seconds before using this command again.",
  "HorseExistsMessage": "You already have a horse. Use /gethorse to retrieve it or /removehorse to remove it.",
  "HorseCreatedMessage": "Your horse has arrived!",
  "NoHorseToRetrieveMessage": "You do not have a horse to retrieve.",
  "MountedMessage": "You cannot use this command while mounted.",
  "OtherPlayerMountedMessage": "Someone is mounted on your horse. You cannot retrieve it right now.",
  "HorseMovedMessage": "Your horse has been moved in front of you.",
  "HorseRemovedMessage": "Your horse has been removed."
}
```
