---
layout: docs
title: 3c. Build management
permalink: /docs/3/c-buildmanage/
---
As an admin, you are given powerful tools to manage block placements, deletions, and WorldEdit selections.
Learning to master these tools is important when rolling back grief and restoring other member's builds.

## Using CoreProtect
CoreProtect is a heavy block management tool that provides detailed logs of all blocks placed and removed.
This plugin allows you to make detailed, specific rollbacks and restorations while managing the integrity of our worlds.
You can display an in-game list of the available commands with three aliases:
 * `/coreprotect help` - The default and longest command, only admins can use it.
 * `/core help` - An alias of the default command, only admins can use it.
 * `/co help` - The shortest alias, only admins can use it.

We will demonstrate command usage with the alias `/co`, as it is the shortest and quickest, but all three variants are functional. 

### Block inspection tool
The inspection tool is a toggleable feature that allows you to click any block and view all previous changes made to that specific location.
It will show WorldEdit selections, placements, deletions, and even natural changes such as water or an explosion.
 * `/co inspect` - Toggles the inspector and can be disabled by typing the command a second time.
 * `/co i` - An alias of the previous command and serves the same function.

This tool is mostly used to quickly check for damage such as a deleted build and also displays how long ago a change was made.

### Rolling back a member
Likely the most used tool of this plugin, the rollback feature allows an administrator to roll any member's changes back.
This command will affect just about anything so specifying perimeters is important.
 * `/co rollback` - Performs a rollback depending on the user and time you specify.
 * `/co rb` - An alias of the previous command and serves the same function.

#### Command usage and perimeters
 * `/co rollback u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 * `/co rb u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 
The first three perimeters should be used at all times.
 * `u:<user>` - Specifies a member by their username to rollback.
 * `t:<time>` - Specifies the amount of time to roll a person back.
   <br>
   You can specify weeks (example, `t:1w`), days (`t:2d`), hours (`t:4h`), minutes (`t:10m`), or seconds (`t:5s`).
   <br>
   To be even more specific, you can pick time amounts (example, `t:1d4h`) and use decimals (`t:2.50h`).
 * `r:<radius>` - Specifies a radius, used to only rollback blocks near your location.
   <br>
   You can specify a number (example, `r:5`), a world (`r:flatlands`), or a global rollback (`r:global`).
   <br>
   You can even specify a WorldEdit selection (example, `r:#worldedit` or `r:#we`).

If you want, you can use the latter perimeters to be more specific.
 * `a:<action>` - Restricts the rollback to a certain action.
   <br>
   For example, if you only want to rollback placements, you can use `a:+block`.
 * `b:<blocks>` - Restricts the rollback to certain block types.
   <br>
   For example, if you only want to rollback stone, you can use `b:1`.
   <br>
   You can even specify multiple items, such as `b:1,5,7`.
 * `e:<exclude>` - Excludes certain block types from the rollback.
   <br>
   For example, if you don't want any TNT to come back during a rollback, you can use `e:46`.
   <br>
   You can specify multiple items just like the above perimeter.

Adding a hashtag to the end of your command allows you to perform additional actions. This feature isn't recommended for normal usage.
 * `#<hashtag>` - Performs diagnostic or visual actions.

Here's a list of hashtags you can use.
 * `#preview` - Previews a rollback or restore.
 * `#count` - Returns the number of rows found in a lookup or query.
 * `#verbose` - Displays additional information during a rollback or restore.
 * `#silent` - Displays minimal information during a rollback or restore.

### Restoring a member
The restore feature allows an administrator to bring back a member's placed or removed blocks.
Like a rollback, this command is very powerful so specifying perimeters is important.
 * `/co restore` - Performs a restore depending on the user and time you specify.
 * `/co rs` - An alias of the previous command and serves the same function.
 
#### Command usage
 * `/co restore u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 * `/co rs u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`

> **Tip:** The restore feature has the same options as rollback, so for detailed instructions just refer to the above list of perimeters.

### Looking up a member
This command allows you to search through block data using the same perimeters as `/co rollback` and `/co restore`.
 * `/co lookup` - Performs an advanced block data lookup depending on the user and time you specify.
 * `/co l` - An alias of the previous command and serves the same function.
 
#### Command usage
 * `/co lookup u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 * `/co l u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
   <br>
   If multiple pages are returned, use `/co lookup <page>` to switch pages.
   <br>
   To change the number of lines displayed on a page, use `/co lookup <page>:<lines>`.
   <br>
   For example, `/co l 1:10` will return ten lines of data, starting at the first page.
   
Certain commands like `/co purge` should never be used and an attempt to do so will result in a suspension.
Always keep in mind that proper usage of these commands are your responsibility.

## Using the logstick
When CoreProtect is being flooded or isn't available for whatever reason, administrators have a second way of logging blocks.
The logstick serves as a crude backup and logs block placements and deletions, but it doesn't log WorldEdit selections.

### Obtaining the logstick
 * `/logstick` - Places a wooden stick in your inventory.

After obtaining a wooden stick as an administrator, you can click any block and view logs.
Natural damage such as explosions are not logged and the logs will wipe under a server restart.

### Performing logstick rollbacks
This command will use the gathered logs to rollback a member's actions by their username.
Upon a twenty-four hour ban, the banned member will automatically be rolled back.
> **Note:** This command is depreciated and is only supposed to be used when CoreProtect is unavailable. In some cases this feature will not restore sign data, chest items, or newer blocks.

#### Command usage
 * `/rollback <user>` - Performs a rollback depending on the user you specify.
 * `/rb <user>` - An alias of the previous command and serves the same function.
 
### Reverting logstick rollbacks
This command will undo a recently performed rollback depending on the member's username.
Like the previous command, this function may be incapable of restorting some blocks, items, or data.

#### Command usage
 * `/rollback undo <user>` - Reverts a rollback depending on the user you specify.
 * `/rb undo <user>` - An alias of the previous command and serves the same function.

## Wiping the flatlands
While the flatlands are usually wiped on a monthly basis, Telnet Administrators and above are given the ability to wipe the main world in case of corruption or heavy lag.
This command is only intended for emergency situations where the issue cannot be detected or the server is becoming unresponsive.

#### Command usage
 * `/wipeflatlands` - Wipes the flatlands while restarting the server.

This command can only be used through Telnet or another console.
