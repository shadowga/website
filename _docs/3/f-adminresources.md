---
layout: docs
title: 3f. Admin resources
permalink: /docs/3/f-adminresources/
---
Our server has different tools and resources that can be used to make tasks easier.
If a service hasn't been mentioned anywhere else in the documentation, it's listed here for quick reference.

## File transfer server
Our server for file uploads and downloads (HTTPD) can be used for quick access to certain in-game files.
Accessing our file transfer server requires a specific address and port (`http://b.shadow.ga:27579/`) as it's hosted through Minecraft.

### Navigation
Navigating through the server is fairly easy as each feature can be located using a trailing slash.
Here's a list of valid directories:
 - `/schematic/list` - Views a dynamic list of saved WorldEdit schematics.
 - `/schematic/upload` - Loads an interface for uploading schematics.
 - `/permbans` - Views a plain text copy of our `permbans.yml` list. This includes suspended users.
 - `/players` - Views a plain text list of our currently added administrators; sorted by their rank.
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

### Telnet server
Telnet Admins and higher can use the server's command-line interface for administrating without direct access to the game.
Upon logging in through the telnet service, admins can send commands and view server statistics through a client.
This feature is helpful for portable administration, log checking, and monitoring as it's basically a lightweight server control panel.

### Finding a client
Admins have a wide array of different applications and programs to use as a client for the service.
We recommend using FTC, a lightweight telnet client made for Minecraft servers like this one.
FTC requires a desktop copy of Java to work, but most machines come with the software pre-installed.
To see if you have Java installed on your machine, follow [this guide](https://www.java.com/en/download/help/version_manual.xml).

Once you have made sure that Java is installed, you can download the client by clicking [this link](https://git.io/v7kJw).
Since the program has a `.jar` extension, you can open it using the Java platform.
If you'd rather use something else instead, the Windows operating system provides a built-in client that isn't enabled by default; TechNet (Microsoft) has a guide on that [here](https://technet.microsoft.com/en-us/library/cc771275).

### Using the client
After you have chose and installed a client, you must use the address and port `b.shadow.ga:26579` to connect.
With the recommend client mentioned above, this information can be specified in the 'server' box.
> **Note:** Make sure to seperate the server address (subdomain) and port with a colon. If you forget this step, the client won't be able to properly form a connection.

Keep in mind that the five-digit port can change over time, so check back with this page if it suddenly stops working.
The steps described may be similar or different depending on what client you use.
If you can't get another client to work, use the recommended option or consult your software's developer.
