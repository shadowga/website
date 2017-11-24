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

- `/schematic/list` - Views a dynamic list of saved WorldEdit schematics.
- `/schematic/upload` - Loads an interface for uploading schematics.
- `/permbans` - Views a plain text copy of our `permbans.yml` list. This includes suspended users.
- `/players` - Views a plain text list of our currently added administrators; sorted by their rank.
- `/help` - Views a plain text list of every server command, proper usage, and description.
- `/list` - Similar to the above directory, views an updated list of the server's online members.
 
### Schematic transfer
Using the schematic list (or [downloader](http://b.shadow.ga:27579/schematic/list)), anyone can download a file by clicking on its name.
Only files with a `.schematic` extension can be downloaded and they're sorted alphabetically onto a dynamic list.
New entries to the list can be uploaded with a page refresh.

> **Note:** Don't download the schematics of other people without their permission. Administrators must be added in-game for some transfer features to work properly.

The schematic [uploader](http://b.shadow.ga:27579/schematic/list) can only be used by administrators.
This interface allows you to directly upload a file from your computer.
Files with a size above sixty-four kilobytes will not upload; abuse of this feature is prohibited.

### Archives and backups
Preventing data loss is very important, so we take several measures to prevent that from happening.
If we lose any data, backups of the server and website are handled by the server owner.
[DigitalOcean](https://m.do.co/c/7438217b1bcd) handles our forum and other VPS-related backups.

We periodicially update our archive [repository](https://git.io/v7PUB).
Anyone can download public archives and they currently include our schematics and in-game worlds.
If the repository gets too big, older releases may be deleted but we'll keep private copies of them.

## Telnet server
Telnet Admins and higher can use the server's command-line interface for administrating without direct access to the game.
Upon logging in through the telnet service, admins can send commands and view server statistics through a client.
This feature is helpful for portable administration, log checking, and monitoring as it's basically a lightweight server control panel.

### Finding a client
Admins have a wide array of different applications and programs to use as a client for the service.
We recommend our self-maintained client made for our server, which you can download [here](https://git.io/v7kJw).
If the download isn't working, check to see if [Java](https://www.java.com/en/download) is installed.

Since the program is a binary, you can open it with the Java Runtime Environment (JRE or Java SE JRE).
If you'd rather use something else, the Windows operating system provides a built-in client that isn't present by default; TechNet (Microsoft) provides a [guide](https://technet.microsoft.com/en-us/library/cc771275) on enabling the feature.

### Using the client
After you have chose and installed a client, you must use the address and port `b.shadow.ga:26579` to connect.
With the recommend client mentioned above, this information can be specified in the 'server' box—found on the bottom-left corner.
> **Note:** Make sure to seperate the server address (subdomain) and port with a colon. If you forget this step, the client won't be able to properly form a connection.

Keep in mind that the five-digit port can change over time, so check back with this page if it suddenly stops working.
The steps described may be similar or different depending on what client you use.
If you can't get another client to work, consult the software's publisher or developer.

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

### Other commands
A few other niche plugins can provide cosmetic effects.
Cosmetic features with narrow functionality are listed here.

* `/firework <user>` - Ignites a firework at the specified member's location.
* `/spawncorpse [user]` - Spawns a corpse at your location, your skin by default; if specified, can be the skin of another member.
 
Don't spawn too many corpses because they won't disppear soon.
If a member is killed or dies for some other reason, their corpse will automatically spawn at that point.
