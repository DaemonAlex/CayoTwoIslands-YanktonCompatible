## Cayo Two Islands - North Yankton Compatible

A slimmed-down version of Cayo intended to work with [North Yankton Enabled](https://github.com/alberttheprince/NorthYankton/). Files used with North Yankton have been restored, and if you'd like to be able to use North Yankton with Cayo, then choose this. If you are not interested in using North Yankton, please use [The Unedited Upload](https://github.com/alberttheprince/CayoTwoIslands). I have removed some things I felt were unnecessary (personal opinion stylistically) and will make additional changes so things like ped traffic don't interfere with North Yankton's traffic and vice versa.

Based initially on Tay's Cayo Two Islands, this project was continued following the deletion/selling of the original open-source resource.


# CayoTwoIslands 🏝️

Designed for RP and exploration in mind, CayoTwoIslands does everything [Cayo Improvements](https://github.com/TayMcKenzieNZ/CayoImprovements) does, except one important and highly requested feature; no more concealment.

---------------------------------------


 CayoTwoIslands enhances the island by removing obstructing collisions, adds more vegetation, street lights, heist props and socializing opportunities.

**This resource is for FiveM usage with the understanding that you will not modify, sell or reupload elsewhere without my permission.**

It is to work alongside [[pmms](https://github.com/kibook/pmms)] for playing content on the TV screens, as well as [[fivem-scenarios](https://github.com/kibook/fivem-scenarios)] for interacting with scenarios around the world, (like seats and scenarios) including Cayo Perico.

This is a passion project of mine that began in December of 2020 to self teach myself Codewalker and has been constantly updated and developed since.

Screenshots are provided in their respective folder.


I hope you enjoy 😊

---------------------------------------

# **REQUIREMENTS** ⚙️

- **Latest recommended artifacts** [for Windows](https://runtime.fivem.net/artifacts/fivem/build_server_windows/master/) **or** [for Linux](https://runtime.fivem.net/artifacts/fivem/build_proot_linux/master/)

-  [Gamebuild 2189 or higher](https://forum.cfx.re/t/tutorial-forcing-gamebuild-to-casino-cayo-perico-or-tuners-update/4784977)

- [Poodle Multimedia Script](https://github.com/kibook/pmms) **for the TV at the Beach Party.** 

> By default, PMMS is set to admin only 
> access, you can change this in the 
> permissions.cfg provided with it, if you 
> would prefer all players can access it.
>
> you will need to read pmms installation 
> instructions on the GitHub repository, and if you
> can't figure it out, open an issue. 
>
> I'm **not** here to hold your hand.

---------------------------------------

# Configuring PMMS 

**Please see [Kibook's PMMS](https://github.com/kibook/pmms) for installation instructions and troubleshooting**

------------------


# Static Emitters 🎶

I have disabled the static emitters at the Arena Wars location, however if you are using PMMS alongside my Cayo Perico resource, PMMS disables static emitters when media is being rendered, and reenables them when the media has stopped playing, therefore, it counteracts with this resource. 

To 'fix' this, open the `staticEmitters.lua` file inside the PMMS resource, and set the following to false like so;

```
{name = "SE_DLC_AW_Arena_Crowd_Background_Main", enabled = false},
{name = "SE_DLC_AW_xs_arena_VIP_Radio", enabled = false},
{name = "SE_DLC_AW_xs_x18_int_mod_garage_radio", enabled = false},
{name = "SE_DLC_AW_xs_x18_int_mod2_garage_radio", enabled = false},
```
---------------------------------------

# CONTENTS 🏝️

- Spawns Cayo Perico alongside Los Santos!

- Working lighthouse

- **Heist props**  - Can be changed in the `entitysets.lua` file within the **scripts** folder

- Removed snow falling from North Yankton 🌨️

- Runway lights and a helipad

- Street lights around the main roads of the island

- Mansion Pool improvement and solid sun loungers, beach ball, floatie, tables and chairs

- Mansion entrance gate doors removed for access

- Side doors of mansion compound opened and lift doors removed for your teleporter script convenience

- Animal cage doors opened - I will **not** be providing doorlock support **#cringe**

- Illuminated Boat Shed near party area and beached whale

- Illuminated skull near grave, opposite party area

- Illuminated beach party area with buoys, DJ stand lights, bar lights and TVs

- Deleted and opened underwater gate below El Rubio's mansion

- Deleted all sea mines -- Want them back? Delete **h4_islandx_sea_mines** from the `ymap` folder.

- Removed invisible collisions

- Removed invisible collision at Beach DJ Booth

- Junk cleanup

- Opened hangar doors

- Sunken UFO & Loch Ness Monster

- Crashed plane

- Runway clearance lights

- Food stall, shop and Ice Cream parlor

- Vehicles

- NPC Peds -- can be removed or commented out in `peds_config.lua`

---------------------------------------

# BUGS 🐛

- some IPL Loader scripts have the following code:

```lua
LoadMpDlcMaps()
EnableMpDlcMaps(true)
```

This conflicts with Cayo Perico and the hangar, as my resources are already requesting the required IPLs, maps, and entitysets. 

Set it to false and request your IPLs the correct way.

- Player may not be able to move their cursor any further than Cayo Perico, if they are inside any of the interiors on the island, however it seems to fix itself once the player leaves the interior


---------------------------------------

# **HANGAR COLLISIONS: 🛩️**

`Original Hangar Collision` folder provided. If you happen to have the '"[Cayo Perico Shops MLO](https://forum.cfx.re/t/mlo-cayo-perico-shops/1994908)' resource, as well as mine, the server refuses to read the collision file for shops, but instead, read mine, making the shop collisions not work. 

Just copy and paste mine, or the Cayo Perico Shops collision file **(h4_islandairstrip_12)** into the ybn folder. 

---------------------------------------

# Frameworks & Other Cayo Perico Resources / Scripts Support:

I don't use any fancy frameworks or any other Cayo Perico related resources, so you'll have to troubleshoot it on your **own.** These are simply ymap, ytyp and ybn files.

---------------------------------------


# Installation ⚙️: 

* Download repository and put the `CayoTwoIslands` folder in your server files

* Add `h4_islandairstrip_12` from the `Original Hangar Collison` folder, and insert it into `CayoTwoIslands` > `stream` > `ybn` folder. If you are using the Cayo Perico Shops resource, ignore this step

* add `start CayoTwoIslands` to your server.cfg

* Restart server or type `/start CayoTwoIslands` into the chat window 


--------------------

# FAQ 💬

**Q: How can I change what's inside the cabinet in the basement?**

**A:** These are called entitysets and can be changed in the cayo_perico_entitysets.lua file.

------------

**Q: Can I delete, change or turn off the invincible NPC peds on the island?**

**A:** Yes, open peds_config.lua and everything has been configured there. You can add / remove entries, or comment it out from the fxmanifest to completely disable them.

You will also need to comment out main_peds.lua if you want to disable them completely.

------------

**Q: When I use this resource, I can't use Rockstar Editor. Why?**

**A:** This should be fixed, as the Cfx.re team have pushed an update on February 8th 2022 which implemented some CPacketIPL changes for the replay editor. This should fix replay editor issues on build 2189 and above with common IPL loading resources.

Read about it [here](https://forum.cfx.re/t/cfx-re-client-update-fivem-redm-for-february-8th-2022/4813410)

