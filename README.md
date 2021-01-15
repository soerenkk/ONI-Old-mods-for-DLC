# ONI-Old-mods-for-DLC
A way to get older mods to maybe work in the DLC, until the mod maker releases an official update.

**Parts of this guide was copied or have gotten inspired from [Peter Han (peterhaneve)](https://github.com/peterhaneve/ONIMods/blob/main/README.md).**


## Disclaimer
This is a trick, and it doenst work with all mods. With the release of the DLC, some things have changed, and thereby it is probably only a few and simple mods this trick works with.

Bigger and more complex mods may interact with the game code that have been changed, and may (most likely will) result in wierd game experiences or the game crashing.

I nor the mod makers, take **NO** resposibility of ruined maps, faulty/flawed execution of the trick or any other kind. Use of this trick is completely on your own risk.


## Locate or create the "local" mod folder

Steam users: Before trying a local download or reporting an issue, use [Mod Updater](https://steamcommunity.com/sharedfiles/filedetails/?id=2018291283) to see if the mod is out of date.

![Location where local mods should be installed](https://github.com/peterhaneve/ONIMods/blob/main/Docs/localmods.png)
Image sourced by: [Peter Han (peterhaneve)](https://github.com/peterhaneve/ONIMods/blob/main/README.md)

* Windows: `%USERPROFILE%\Documents\Klei\OxygenNotIncluded\mods\local`
  Replace the documents path with the path to your `Documents` folder if this folder has been redirected.
* Mac OS: `/Users/user name/Library/Application Support/unity.Klei.Oxygen Not Included/mods/Local`
  Replace `user name` with your user name.
* Linux: `~/.config/unity3d/Klei/Oxygen Not Included/mods/Local`

**If the "local" folder isnt present, then create it yourself.**

**Do not use a Steam copy and a local copy of the same mod at the same time.** Disable the Steam version in the mods list before activating any local copies.


## Locate the mod you want

The mod you already have installed from Steam, will be located in a folder in the "Steam" folder in the "mods" folder.

![Location where Steam mods should be installed](https://github.com/peterhaneve/ONIMods/blob/main/Docs/steammodsfolder.png)
Image sourced by: [Peter Han (peterhaneve)](https://github.com/peterhaneve/ONIMods/blob/main/README.md)

* Windows: `%USERPROFILE%\Documents\Klei\OxygenNotIncluded\mods\Steam`
  Replace the documents path with the path to your `Documents` folder if this folder has been redirected.
* Mac OS: `/Users/user name/Library/Application Support/unity.Klei.Oxygen Not Included/mods/Steam`
  Replace `user name` with your user name.
* Linux: `~/.config/unity3d/Klei/Oxygen Not Included/mods/Steam`

In the "Steam" mod folder, the folder of the actual mod is located. This folder is named with a number, in my case, I wanted to do this for the mod "Pliers". In my Steam folder that mod folder was named "1848884654".


Then copy the mod folder to your "local" mod folder, and then rename the folder to the mod name (the name of the ".dll" file (or what is used on Mac/Linux)).


When the folder is copied from the Steam mod folder to the local folder, and renamed. Then you have to add the following file to the renamed folder:

[mod_info.yaml](mod_info.yaml)



## Lastly
Once that is done, you just have to open steam, start ONI, go to mods and enable the mod(s) you want to play with.

Once the mods on steam gets updated, you should disable and preferebly delete the mod from the local mod folder, and use the mod from steam, since the mods in the local mod folder wont get any updates.
