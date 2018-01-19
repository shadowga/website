---
layout: docs
title: c. Resources
permalink: /docs/2/c-resources/
---
Our server has different tools and resources that can be used to make tasks easier.
If a service hasn't been mentioned anywhere else in the documentation; it's listed here for quick reference.

## File transfer server
Our server for file uploads and downloads (HTTPD) can be used for quick access to certain in-game files.
You can directly access the online file transfer server by manually entering an address and port (`b.shadow.ga:27579`) or through [this link](http://b.shadow.ga:27579).

> **Note:** That address alone will produce an error because you aren't requesting anything yet. You'll need to get somewhere by navigating through the server.

### Navigation
Navigating through the server is fairly easy as each feature can be located using a trailing slash.
Here's a list of trailing slashes you can use:

- [`/schematic/list`](http://b.shadow.ga:27579/schematic/list) - Views a dynamic list of saved WorldEdit schematics.
- [`/schematic/upload`](http://b.shadow.ga:27579/schematic/upload) - Loads an interface for uploading schematics.
- [`/permbans`](http://b.shadow.ga:27579/permbans) - Views a plain text copy of our `permbans.yml` list. This includes suspended users.
- [`/players`](http://b.shadow.ga:27579/players) - Views a plain text list of our currently added administrators; sorted by their rank.
- [`/help`](http://b.shadow.ga:27579/help) - Views a plain text list of every server command, proper usage, and description.
- [`/list`](http://b.shadow.ga:27579/list) - Similar to the above directory, views an updated list of the server's online members.
 
### Schematic transfer
Using the schematic list (or [downloader](http://b.shadow.ga:27579/schematic/list)), anyone can download a file by clicking on its name.
Only files with a `.schematic` extension can be downloaded and they're sorted alphabetically onto a dynamic list.
New entries to the list can be uploaded with a page refresh.

> **Note:** Don't download the schematics of other people without their permission. Administrators must be added in-game for some transfer features to work properly.

The schematic [uploader](http://b.shadow.ga:27579/schematic/upload) can only be used by administrators.
This interface allows you to directly upload a file from your computer.
Files with a size above sixty-four kilobytes will not upload; abuse of this feature is prohibited.

## Telnet server
Telnet Admins and higher can use the server's command-line interface for administrating without direct access to the game.
Upon logging in through the telnet service, admins can send commands and view server statistics through a client.

### Client usage
Admins have a wide array of clients to use for the service.
We recommend our self-maintained [Java](https://www.java.com/en/download)-based client made for our server, which you can download [here](https://git.io/v7kJw).
If you'd rather use something else, Windows has a built-in client you can [enable](https://technet.microsoft.com/en-us/library/cc771275).

> **Note:** Make sure to seperate the server address (subdomain) and port with a colon. If you forget this step, the client won't be able to properly form a connection.

After you have chose and installed a client, you must use the address and port `b.shadow.ga:26579` to connect.
Keep in mind that the five-digit port can change over time, so check back with this page if it suddenly stops working.

### Telnet commands
The telnet server provides some built-in commands that can manage the server and your connection.
These commands can only be used through telnet; they won't work in-game.

> **Note:** Some actions capable with this resource can result in server downtime. Work with this feature carefully and avoid syntax mistakes.

* `telnet.help` - Provides a list of management commands and their functions.

#### Command usage
Here's a developed list of telnet commands you can use.
They shouldn't be prefixed with a slash (`/`) like conventional in-game commands.

* `telnet.stop` - Shuts down the server; this doesn't restart.
* `telnet.log` - Toggles between three filters - all logs, only chat logs, and only non-chat logs.
* `telnet.exit` - Terminates your connection to the telnet server.

## Control panel
Providing a similar service to Telnet, Executive administrators utilise the [PufferPanel game management panel](https://www.pufferpanel.com/) to manage the state of the server or execute console-level commands. The control panel also offers a file-transfer option, to manage files running on the server.

### Usage and access
To access the panel, navigate to [p.shadow.ga](https://p.shadow.ga) and sign-in using the credientials given. Once signed-in, users should select "shadow.ga" in order to manage the server. 

## Cosmetics
Several cosmetic plugins are installed to provide features that accompany building, texture, and overall experience.
Many of these tools can have an extensive amount of functions, so mastering them may take some time.

* `/pp help` - Provides help for functions related to particles. Use tab to fill in syntax.
* `/chimney` - Without arguments, provides help for functions related to chimney particles.

### Embedded particles
A given amount of particles can be embedded, meaning they'll adhere to the member applying them.
These particles serve as an effect or aura; they're also great for customisation.

* `/pp effects` - Provides a list of effects (or particle styles) you can use on the following command.
* `/pp styles` - Provides a list of styles you can use on the following command.
 
#### Command usage
Once you have viewed a list, pick an effect or style you'd like to apply.
Styles can only be applied after you've chosen an effect.

* `/pp effect <effect>` - Applies an effect, dynamically bound to your position.
* `/pp style <style>` - Applies a style, accompanying the effect chosen earlier.
 
### Stationary particles
Particles that are stationary (or fixed) will be embedded to a set of coordinates, rather than a member.
These particles are great for buildings and functionally-appearing interiors.

> **Note:** The modification of these particles is currently restricted to Senior Admins and higher. This is to prevent server lag, possible client lag, and secure the feature from unwanted usage.

* `/pp fixed` - Provides information on the usage of stationary particles.

#### Command usage
Identifications are used by the plugin for specifying a certain set of stationary particles.
They are presented in numbers.

* `/pp fixed list` - Provides a list of existing sets with their identifications.
* `/pp fixed info <id>` - Provides information on a specific set of particles.

The following commands are self-explanatory.
They're capable of creating and removing sets of stationary particles.

* `/pp fixed create <x> <y> <z> <effect> <style> [data]` - Creates a new identification (or set) of stationary particles.
   <br>
   This command relies on coordinates to determine the location you'd like.
   <br>
   If you'd like the set created at your present location, use `~` to replace `<x>`, `<y>`, and `<z>`.
* `/pp fixed remove <id>` - Removes a set of stationary particles by identification.
   <br>
   You can only remove sets of particles created under your username.

### Chimney particles
Senior Admins and higher can apply chimney particles to builds.
They're stationary and operate vertically, making them more suitable for fireplaces and different arrays.

* `/chimney <tgt | std>` - Creates a chimney particle array.
   <br>
   The `tgt` option will create an array where you're aiming; `std` will create an array where you're standing.

### Spawning mobs
Anyone can spawn mobs in using a set of commands.
Spawning too many mobs can lag or crash the server; that can lead to a ban.

> **Note:** Mobs can only be removed from the console, so the only other way to get rid of a mob you've spawned is by killing it.

 * `/smob` - With the correct arguments, spawns mobs.
 * `/sm` - An alias of the previous command and serves the same function.
 * `/smob help` - Provides help for functions related to spawning mobs.
 * `/smob list` - Provides a list of mobs you can spawn.

#### Command usage
With the proper arguments, you can customise the mobs spawned.
Both natural and player-made sequences can be emulated with this feature.

 * `/smob <mob> [amount]` - Basic command; spawns a mob. Use `amount` to spawn multiple mobs.
 * `/smob <mob>;<mob> [amount]` - With a semicolon, allows you to spawn stacked mobs.
 * `/smob <mob> [amount] <coordinates>` - Allows you to spawn mobs at a set of coordinates.

### Image maps
This feature lets you put any image you'd like onto the map of your choice.
From there, you can place the map in an item frame (for public display) or keep it a secret.

> **Note:** If you'd like to draw an image onto a blank map, you must right-click it first (the map must be pre-loaded before you use `/drawimage`).

 * `/drawimage [link]` - Draws an image onto the map in your hand. Source link must end in an image extension (`.png`, `.jpg`, etc).

### Other commands
A few other niche plugins can provide cosmetic effects.
Cosmetic features with narrow functionality are listed here.

* `/chairs <on | off>` - Enables or disables client-side chairs; it's on by default.
* `/firework <user>` - Ignites a firework at the specified member's location.
* `/spawncorpse [user]` - Spawns a corpse at your location, your skin by default; if specified, can be the skin of another member.
 
Don't spawn too many corpses because they won't disppear soon.
If a member is killed or dies for some other reason, their corpse will automatically spawn at that point.
