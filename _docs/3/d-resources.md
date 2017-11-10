---
layout: docs
title: 3d. Resources
permalink: /docs/3/d-resources/
---
Our server has different tools and resources that can be used to make tasks easier.
If a service hasn't been mentioned anywhere else in the documentation; it's listed here for quick reference.

## File transfer server
Our server for file uploads and downloads (HTTPD) can be used for quick access to certain in-game files.
You can directly access the online file transfer server by manually entering an address and port (`b.shadow.ga:27579`) or through [this link](http://b.shadow.ga:27579).
That address alone will produce an error because you aren't requesting anything yet.

### Navigation
Navigating through the server is fairly easy as each feature can be located using a trailing slash.
Here's a list of trailing slashes you can use:
 - `/schematic/list` - Views a dynamic list of saved WorldEdit schematics.
 - `/schematic/upload` - Loads an interface for uploading schematics.
 - `/permbans` - Views a plain text copy of our `permbans.yml` list. This includes suspended users.
 - `/players` - Views a plain text list of our currently added administrators; sorted by their rank.
 - `/help` - Views a plain text list of every server command, proper usage, and description.
 - `/list` - Similar to the above directory, views an updated list of the server's online members.
 
### Downloading schematics
Using the schematic list, anyone can download a file by clicking on its name.
Only files with a `.schematic` extension can be downloaded using the interface for security reasons.
Files are sorted alphabetically onto a dynamic list that can be updated by a page refresh.
Don't download other's entries without their permission.

### Uploading schematics
The interface for uploading can only be used by locations that are added in-game as an admin, meaning only administrators can use this feature.
When uploading a schematic, the 'choose file' option allows you to pick a file from your computer and upload it to the server.
Files with a size above sixty-four kilobytes will not upload and inappropriate file names aren't allowed.

## Archives and backups
Preventing data loss is very important, so we take several measures to prevent that from happening.
If we lose any data, backups of the server and website are kept through both public and private means.
Members can even download parts of the server if something is lost.

### Downloading archives
We periodically archive some contents to a GitHub repository [here](https://git.io/v7PUB).
From there, anyone can download archives from latest to oldest.
Right now we only allow public backups of our schematics and in-game worlds.
If the repository gets too big, older releases may be deleted to free up space.

### Server backups
The entire server is often backed up to private storage.
While we don't allow downloads of our entire server, you can request a specific file from us.
Private backups are handled by the server owner and requests are fulfilled at their discretion.

### Website backups
Our homepage and documentation are handled through a public repository.
Forum backups are handled by DigitalOcean and we keep them private.
If we experience problems with the forum, we can restore to a number of snapshots.

## Telnet server
Telnet Admins and higher can use the server's command-line interface for administrating without direct access to the game.
Upon logging in through the telnet service, admins can send commands and view server statistics through a client.
This feature is helpful for portable administration, log checking, and monitoring as it's basically a lightweight server control panel.

### Finding a client
Admins have a wide array of different applications and programs to use as a client for the service.
We recommend our self-maintained client made for our server, which you can download [here](https://git.io/v7kJw).
If the download isn't working, check to see if [Java](https://www.java.com/en/download) is installed.

Since the program is a binary, you can open it with the Java Runtime Environment (JRE or Java JRE).
If you'd rather use something else, the Windows operating system provides a built-in client that isn't present by default; TechNet (Microsoft) provides a [guide](https://technet.microsoft.com/en-us/library/cc771275) on enabling the feature.

### Using the client
After you have chose and installed a client, you must use the address and port `b.shadow.ga:26579` to connect.
With the recommend client mentioned above, this information can be specified in the 'server' box—found on the bottom-left corner.
> **Note:** Make sure to seperate the server address (subdomain) and port with a colon. If you forget this step, the client won't be able to properly form a connection.

Keep in mind that the five-digit port can change over time, so check back with this page if it suddenly stops working.
The steps described may be similar or different depending on what client you use.
If you can't get another client to work, consult the software's publisher or developer.
