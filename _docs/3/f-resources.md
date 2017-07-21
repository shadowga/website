---
layout: docs
title: 3f. Resources
permalink: /docs/3/f-resources/
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
When uploading a schematic, the 'choose file' button allows you to pick a file from your computer and upload it to the server.
Files with a size above sixty-four kilobytes will not upload and inappropriate file names aren't allowed.

## 
