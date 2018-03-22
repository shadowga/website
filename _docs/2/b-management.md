---
layout: docs
title: b. Management
permalink: /docs/2/b-management/
---
As an admin, you are given powerful tools to manage block placements, deletions, and WorldEdit selections.
Learning to master these tools is important when rolling back grief and restoring a member's builds.

## Using CoreProtect
CoreProtect is a heavy block management tool that provides detailed logs of all blocks placed and removed.
You can display an in-game list of the available options with three main commands:

 * `/coreprotect help` - The default and longest command, only admins can use it.
 * `/core help` - An alias of the default command, only admins can use it.
 * `/co help` - The shortest alias, only admins can use it.

We will demonstrate command usage with the alias `/co`, as it is the shortest and quickest, but all three variants are functional. 

### Block inspection tool
The inspection tool is a toggleable feature that allows you to click any block and view all previous changes made to that specific location.
It will show WorldEdit selections, placements, deletions, and even natural changes such as water or an explosion.

 * `/co inspect` - Toggles the inspector, can be disabled by typing the command a second time.
 * `/co i` - An alias of the previous command and serves the same function.

This tool is mostly used to quickly check for damage such as a deleted build and also displays how long ago a change was made.

### Rolling back a member
Likely the most used tool of this plugin, the rollback feature allows an administrator to roll a member's changes back.
This command will affect just about anything so specifying perimeters is important.

 * `/co rollback` - Performs a rollback depending on the user and time you specify.
 * `/co rb` - An alias of the previous command and serves the same function.

#### Command usage and perimeters
 * `/co rollback u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`
 * `/co rb u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`
 
The first three perimeters should be used at all times.
 * `u:<user>` - Specifies a member by their username to rollback.
   <br>
   Instead of a member, you can specify blocks such as water (`u:#water`), lava (`u:#lava`), sand (`u#sand`), or an explosion (`u:#tnt`).
   
 * `t:<time>` - Specifies the amount of time to roll a person back.
   <br>
   You can specify weeks (example, `t:1w`), days (`t:2d`), hours (`t:4h`), minutes (`t:10m`), or seconds (`t:5s`).
   <br>
   To be even more specific, you can pick time amounts (example, `t:1d4h`) and use decimals (`t:2.50h`).
   
 * `r:<radius>` - Specifies a radius, used to only rollback blocks near your location.
   <br>
   You can specify a number (example, `r:5`), a world (`r:#flatlands`), or a global rollback (`r:#global`).
   <br>
   You can even specify a WorldEdit selection (example, `r:#worldedit` or `r:#we`).

If you want, you can use the latter perimeters to be more specific.
 * `a:[action]` - Restricts the rollback to a certain action.
   <br>
   For example, if you only want to rollback placements, you can use `a:+block`.
   
 * `b:[blocks]` - Restricts the rollback to certain block types.
   <br>
   For example, if you only want to rollback stone, you can use `b:1`.
   <br>
   You can even specify multiple items, such as `b:1,5,7`.
   
 * `e:[exclude]` - Excludes certain block types from the rollback.
   <br>
   For example, if you don't want any TNT to come back during a rollback, you can use `e:46`.
   <br>
   You can specify multiple items just like the above perimeter.

Adding a hashtag to the end of your command allows you to perform additional actions. This feature isn't recommended for normal usage.
 * `#[hashtag]` - Performs diagnostic or visual actions.

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
 * `/co restore u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`
 * `/co rs u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`

> **Tip:** The restore feature has the same options as rollback, so for detailed instructions just refer to the above list of perimeters.

### Looking up a member
This command allows you to search through block data using the same perimeters as `/co rollback` and `/co restore`.

 * `/co lookup` - Performs an advanced block data lookup depending on the user and time you specify.
 * `/co l` - An alias of the previous command and serves the same function.
 
#### Command usage
 * `/co lookup u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`
 * `/co l u:<user> t:<time> r:<radius> a:[action] b:[blocks] e:[exclude]`
   <br>
   If multiple pages are returned, use `/co lookup [page]` to switch pages.
   <br>
   To change the number of lines displayed on a page, use `/co lookup [page]:[lines]`.
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

### Protecting land
Administrators can protect land, however operators won't be able to modify that protected land afterwards.
They're given labels for identification.

> **Note:** WorldEdit and other tools can still bypass this filter, so you'll still need to administrate; although protected land will not interfere with any CoreProtect services.

 * `/protectarea` - Provides a list of functions when ran without arguments.
 
#### Command usage
 * `/protectarea add <label> <radius>` - Creates a protected area with label. Max radius is fifty.
 * `/protectarea remove <label>` - Removes a protected area.
 * `/protectarea list` - Lists all protected areas by their label names.
 
> **Note:** Similar to schematic names, a protected area created with an identical label will overwrite the pre-existing area. Because of this, use unique label names.

 * `/protectarea clear` - Clears all protected areas; console-only function.

## Wiping the flatlands
While the flatlands are usually wiped on a monthly basis, Telnet Administrators and above are given the ability to wipe the main world in case of corruption or heavy lag.
This command is only intended for emergency situations where the issue cannot be detected or the server is becoming unresponsive.

#### Command usage
 * `/wipeflatlands` - Wipes the flatlands while restarting the server.

This command can only be used through Telnet or another console.

## Managing Async
AsyncWorldEdit (AWE) is an addition to WorldEdit that allows for larger edits without lagging the server.
Seniors and higher are capable of viewing, purging, and cancelling member's edits in the queue.
You can display an in-game list of the available options with the following main command:

 * `/awe help` - The default command, only Senior Admins and higher can use it.

### Viewing edit jobs
This command allows you to view a personal or global updated list of the queued block operations.

 * `/awe jobs` - Displays queued block operations.
 
#### Command usage
 * `/awe jobs [page]` - Displays a list of your queued block operations.
 * `/awe jobs u:<user> [page]` - Displays a list of another member's block operations.
 * `/awe jobs all [page]` - Displays a global list of the server's queued block operations.
 
The `[page]` option can be used to specify different pages in numbers, such as `2` for the second page or `10` for the tenth.

### Cancelling edit jobs
This command allows you to cancel specific edits.

 * `/awe cancel` - Cancels queued block operations.
 
#### Command usage
 * `/awe cancel <#id>` - Cancels one of your queued edits depending on the operation ID.
 * `/awe cancel u:<user> <#id>` - Cancels one of another member's queued edits depending on the operation ID.
 
The `<#id>` option (operation ID) is required as it specifies which edit should be canceled.
You can find a specific ID by viewing jobs for yourself, another member, or the server.
 
### Purging edit jobs
This command is similar to the above one except it will cancel every edit in a member's queue or globally.
Admins should only use this command in emergencies as it can cause a major change.

 * `/awe purge` - Purges all queued block operations.

#### Command usage
 * `/awe purge` - Without any other arguments, purges all of your queued operations.
 * `/awe purge u:<user>` - Purges all of a specific member's queued operations.
 * `/awe purge all` - Purges all queued operations on the server.
  
### Toggling Async
Async (AWE) is enabled by default but this command can disable or re-enable the feature.
With Async disabled, edits will be performed without lag prevention.

> **Note:** This command is not recommended without given permission of an Executive or higher.
> It can potentially result in selections becoming unresponsive or abnormally slow.

 * `/awe toggle` - Disables or enables the AsyncWorldEdit service.
 
#### Command usage
 * `/awe toggle` - Without any other arguments, toggles the service on or off.
 
 * `/awe toggle on` - Enables the Async service.
 * `/awe toggle off` - Disables the Async service.
