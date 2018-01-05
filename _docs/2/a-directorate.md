---
layout: docs
title: a. Directorate
permalink: /docs/2/a-directorate/
---
Having an effective and reliable team is imperative, and that's why we carefully manage our administrators.
Some admins manage more than others depending on their ability; a ranking system is used for institution.

## Hierarchy
Having a hierarchy of ranks is a great way of classifying our community, although the two should not be confused as they carry important differences.
Knowing our various ranks allows members to identify and communicate with administrators easily.

---

<div style="text-align: center; margin-top: 15px;"><img src="https://shadow.ga/img/svg/admins.svg"></div>

---

### Super Admins
Super Admins are the basic administrators. They are given banning and smiting abilities, and full access to grief logging plugins. Super Admins are allowed to use some commands that are blocked for operators such as `/tpo` and `/say`.

#### Rank management
Telnets and above can add members to administrator through any console; Seniors and above are capable of adding and removing administrators, but they should do it legally.

 * `/saconfig list` - Lists (already added) administrators by username.
 * `/saconfig info <user>` - Provides additional information on an admin (`<user>`).

> **Note:** Adding members that aren't listed on the admin [roster](https://f.shadow.ga/d/5-list-of-administrators-11-2017) is considered rogue activity. Administrators should learn this command before attempting to use it.

 * `/saconfig add <user>` - Adds a member to administrator, default appointment is Super Admin. For Telnets and above.
 * `/saconfig remove <user>` - Removes a member from administator. For Seniors and above.

### Telnet Admins
Telnet Admins are given the same commands as Super Admins except they can use [telnet](https://shadow.ga/docs/2/c-resources/#telnet-server). Our telnet server allows members with the rank to administrate even when they are not on Minecraft.

#### Appointing members
When a member is officially listed for promotion, Seniors and above can set their rank through any console. Like general management, only do this if they're listed for it. They can also be appointed downwards.

 * `/saconfig setrank <user> telnet_admin` - Appoints an administrator to Telnet Admin.
 * `/saconfig setrank <user> super_admin` - Appoints an administrator back to Super Admin.
 * `/saconfig reload` - Reloads the administrator registry, don't run this too often.

### Senior Admins
Senior Admins have all the abilities as the above ranks. They're also given extra commands that are blocked to lower ranks; like `/summon` and `/socialspy`. The Senior Admin rank is also required for non-applicable ranks, such as Executive and Developer.

#### Appointing members
Telnets can be appointed to the Senior rank using the same method. Unless they were previously removed, we recommend that only Executives perform appointments intended to promote admins.

> **Note:** You can add Super Admins directly to Senior; the command can skip a rank and perform the same operation. It also works vice-versa, as you can demote while skipping a rank.

 * `/saconfig setrank <user> senior_admin` - Appoints an administrator to Senior Admin.
 * `/saconfig setrank <user> <telnet_admin | super_admin>` - Appoints an administrator back to Telnet or Super.

### Executive Admins
Executives are in charge of all lower positions; they have the ability to suspend administrators and market the service. You probably won't see these admins in-game as often because they also take care of platforms like the forum.

## Appointment
We always keep an eye out for potential administrators as the server grows.
While there are different ranks of admin, they all have one thing in common and that is to be reliable and helpful.
This is why candidates for the position are hand-picked based on how they present themselves to everyone.
Here's what we look for:
* The ability to act mature and professional in difficult situations.
* Maintained control over problems when put under heavy stress by other members.
* Knowledge of our rules and helpfulness to inexperienced newcomers.
* Activity and membership on all of our platforms (on and off the server).
* The tendancy to stay out of trouble and remain honest at all times.
* Members who go out of their way to improve other people's experiences.
* Good communicators, people who know the English language well and can talk to people clearly.

If the above sounds like you, make sure to let us know.
Maybe that description reminds you of someone else?
If so, you can directly message an admin to recommend them.

### Selecting members
If you're already an administrator; you can select a member for the position.
Selected members are expected to stand out from everyone else and meet all of the above requirements.
By selecting a member, you agree that they represent a model candidate in your eyes and bring a higher-ranked admin's attention to the member.
We have a few requirements for selection:
* An administrator can only select one member per year.
* The member must meet all qualities of our selection checklist (shown above).
* The member must have not been banned (accidental bans don't count) on the server or forum for at least twenty days or has made a valid appeal for each ban they received.
* The member must have a forum account with two-factor auth enabled.
* The member must have a Discord account connected to our guild, also with two-factor auth enabled.

### Commencing selection
To choose a member, they must agree to become an admin and vow to fulfill all tasks expected of them.
Once you have chosen someone you want to select, you can directly message an Executive or higher and they will the make decision to appoint them or not.

## Management
As mentioned earlier, we organise our staff so members can go to the right person for help.
Depending on what someone wants to administrate or how they perform, they can be promoted or demoted.

### Promoting an admin
When admins further improve themselves, the owner can issue a promotion to them which will up their position in the administrator hierarchy.

This usually occurs when a higher-ranking admin resigns or is placed inactive, opening the opportunity for a promotion.
When we need to promote someone, we usually look for three things; experience, helpfulness, and activity.

### Demoting an admin
Promotions can also work the other way around, as admins can be demoted back to a lower rank as a punishment or to better organise the team.

Executives are capable of demoting or suspending administrators if they've broken the conduct policy, acted improperly, or failed to do their job.
Demotions can also be a result of inactivity and an admin can have themselves demoted on request.
