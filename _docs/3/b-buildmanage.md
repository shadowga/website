---
layout: docs
title: 1b. Build management
permalink: /docs/1/b-buildmanage/
---
As an admin, you are given powerful tools to manage block placements, deletions, and WorldEdit selections.
Learning to master these tools is important when rolling back grief and restoring other member's builds.

## Using CoreProtect
CoreProtect is a heavy block management tool that provides detailed logs of all blocks placed and removed.
This plugin allows you to make detailed, specific rollbacks and restorations while managing the integrity of our worlds.
You can display an in-gamel list of the available commands with three aliases:
 * `/coreprotect help` - The default and longest command, only admins can use it.
 * `/core help` - An alias of the default command, only admins can use it.
 * `/co help` - The shortest alias, only admins can use it.

We will demonstrate command usage with the alias `/co`, as it is the shortest and quickest, but all three variants are functional. 

### Block inspection tool
The inspection tool is a toggleable feature that allows you to left-click a block and view all previous changes made to that specific location.
It will show WorldEdit selections, placements, deletions, and even natrual changes such as water or an explosion.
 * `/co inspect` - Toggles the inspector and can be disabled by typing the command a second time.
 * `/co i` - An alias of the previous command and serves the same function.

This tool is mostly used to quickly check for damage such as a deleted build and also displays how long ago a change was made.
