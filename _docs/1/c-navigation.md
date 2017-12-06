---
layout: docs
title: c. Navigation
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
You can build anything anywhere in this world; it only wipes if the map gets too big, is corrupted, or has been ruined.
 * `/spawn` - Teleports a player to the spawn (in the flatlands).
 * `/flatlands` - Teleports a player to the flatlands.

### Primary worlds
Primary worlds (roughlands, netherlands, enderlands) are places you don't naturally spawn in, but can access using commands.
These worlds will only wipe if they're corrupted and members can build here, just like the flatlands.

The roughlands includes natural biomes—such as deserts, prairies, and jungles; rough areas are great for constructing landscapes or cities.
The netherlands (or nether world) contains an endless set of red platforms, with fire and lakes of lava.

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
 * `0` - To the roughlands. Direct is `/roughlands`.
 * `1` - To the netherlands. Direct is `/nether`.
 * `2` - To the enderlands. Direct is `/ender`.
 * `3` - To the flatlands. Direct is `/flatlands` or `/spawn`.
 * `4` - To the adminworld. Only admins can do this. Direct is `/adminworld` or `/aw`.

### Adminworld
The adminworld is a private world that only Super Admins and above can go in.
On occasion, an admin can invite someone as a "guest", allowing them to join the adminworld for a small amount of time until the server restarts.
When operators are not invited as guests, they can't enter.

 * `/adminworld` - Teleports an administrator to the adminworld.
 * `/aw` - An alias of the previous command and serves the same function.

## Location
Our server uses the basic Essentials kit of commands.
As a result, you can bookmark a set of coordinates both for the public and as a private home.

### Using warps
A warp is a keyword that allows anyone to teleport to a set of coordinates.
Warps are public and can be viewed by anyone, and they can also be overridden.

 * `/warps` - Provides a list of existing warps.
 * `/warp <warp>` - Allows you to... warp to a warp. (Sounds weird, right?)
 
### Using homes
Members can set their own home, which is just like a private warp.
Homes won't appear in the public list of warps and they're good for referencing locations.

> **Note:** Unlike warps, members can't go to homes set by others. They're specific to whoever has set them previously. If you'd like to have a public keyword, you should be using warps instead.

 * `/homes` - Provides a list of your homes.
 * `/home <home>` - Takes you home to a home. (Slightly less weird.)

## Dynamic map
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
The resource pack is an open-source project and we use a repository for easy editing and the ability to quickly make changes; from which you can [obtain](https://github.com/shadowga/resourcepack/archive/master.zip) the latest version.

### Installation
After successfully downloading the resource pack, you can install and activate it normally.
It may take up to a minute for your game to initialize the textures, and then you should be returned to the options menu.
You have now completed all the steps and your resource pack should be working.
