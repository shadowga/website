---
layout: docs
title: 1c. Navigation
permalink: /docs/1/c-navigation/
---
We have different types of worlds so members may choose any environment they like.
While every world shares the same set of guidelines, they can help distinguish the atmosphere and design of builds.
Different worlds are also great for activities such as melee or architect competitions.

## Switching worlds
Worlds can be switched by any member.
To do this, we have the command `/world`, which allows you to specify different types of worlds to visit.
Most worlds have a custom alias command that teleports you there. Different types of worlds can be accessed by different types of members.

### Default world
The default world (flatlands) is where you spawn in upon death or as a new player.
You can build anything anywhere in this world; it only wipes if the map gets too big, is corrupted, or has been badly griefed.
 * `/spawn` - Teleports a player to the spawn (in the flatlands).
 * `/flatlands` - Teleports a player to the flatlands.

### Primary worlds
Primary worlds (roughlands, netherlands, enderlands) are places you don't naturally spawn in, but can access using commands.
These worlds will only wipe if they're corrupted and members can build here, just like the flatlands.

The roughlands includes natural biomes - such as deserts, prairies, and jungles.
Rough areas are great for constructing landscapes or cities, while preserving the nature of whatever you're building.

The netherlands (or nether world) contains an endless set of red platforms, with fire and lakes of lava.
Themic areas fit perfectly in this biome; melee, jumping courses, and fights are great for this world.

The enderlands (or end world) is comprised of little to big islands made out of a light material, with several naturally-occuring platforms.
This place is great for strategy puzzles, mazes, and machinery; you'll find a consistent pale black sky.

#### Command usage
 * `/world <number>` - Teleports a player to the world they specify.
 * `/roughlands` - Teleports a player to the roughlands.
 * `/nether` - Teleports a player to the netherlands.
 * `/ender` - Teleports a player to the enderlands.
 
The first command's perimeter is required.
 * `<number>` - Specifies a world number. Each number (`0` to `4`) takes you somewhere else.

Here's each number and the world it corresponds to.
 * `0` (zero) - To the roughlands. Direct is `/roughlands`.
 * `1` (one) - To the netherlands. Direct is `/nether`.
 * `2` (two) - To the enderlands. Direct is `/ender`.
 * `3` (three) - To the flatlands. Direct is `/flatlands` or `/spawn`.
 * `4` (four) - To the adminworld. Only admins can do this. Direct is `/adminworld`.

### Adminworld
The adminworld is a private world that only Super Admins and above can go in.
It is never wiped, and houses the adminworld village.
On occasion, an admin can invite someone as a "guest", allowing them to join the adminworld for a small amount of time until the server restarts.
When operators are not invited as guests, it is impossible for them to enter this world.
 * `/adminworld` - Teleports an administrator to the adminworld.

## Using Dynmap
Dynmap, as abbreviated in the name, is a dynamic map generator.
This plugin can generate a bird's-eye view of any world through your web browser.
With the online interface, you can also view statistics and use the in-game chat.

### Web interface
The map can be opened like any other webpage [here](http://b.shadow.ga:26589).
From there, it will take you to the default world (flatlands).
By clicking on the arrow to your right, you can select different worlds, switch to different render modes, and view a list of online members.
Chat messages will be displayed at the bottom-left next to the hyperlink button.

On the top-left, you can click on a layer button to filter out certain objects.
Both options are enabled by default and deselecting either one will automatically update the render.
The `markers` option shows where spawnpoints are located and `players` identifies the location of all online members.

### Online chat
If the plugin is able to link your in-game address with that of your connection to Dynmap, you can send and receive messages.
You'll be able to communicate (read and view in-game messages) as if you were on the server through the comfort of a webpage.

Dynmap-sent messages can be distinguished by the `[WEB]` prefix that precedes anything sent through the interface.
Messages sent by members in-game can also show display a text bubble relative to their position on the map; you must be viewing the respective map to use this feature.

### Other information
At the top-center, it will display the Minecraft world-specific time along with an animated representation.
Under the filters button, it will show the world coordinates in relation to where your cursor is located.
The top-right image will display a compass for directional reference.

## Resource pack
Our server uses a custom resource pack that gives builders the ability to add more detail in their creations.
We recommend that all members have it installed.

### Downloading
If the server does not notify you to install the resource pack automatically, you can download and apply it manually.
The resource pack is an open-source project and we use a repository for easy editing and the ability to quickly make changes.
This means that you can obtain the newest version from your browser from [here](https://github.com/shadowga/resourcepack/archive/master.zip).

### Installation
After successfully downloading the resource pack, you can install and activate it normally.
It may take up to a minute for your game to initialize the textures, and then you should be returned to the options menu.
You have now completed all the steps and your resource pack should be working.
