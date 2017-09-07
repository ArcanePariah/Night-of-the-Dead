# Night of the Dead
This repository contains latest version of Night of the Dead for Starcraft II.

## Requirements
1. Starcraft II account (Starter Edition will open the map, but will not let testing it)

## Installation
1. Place bin/src folders in "Mods\Night of the Dead" in Starcraft II install folder (e.g. "C:\Program Files (x86)\StarCraft II\Mods\Night of the Dead"). Create "Mods" folder if necessary.
2. Launch "Mods\Night of the Dead\src\NOTD.SC2Map\ComponentList.SC2Components" to open map in editor. File associations may not work for first run, so be sure to open it with SC2Edit.

## Tips
1. To make map load faster, change Editor startup settings to load triggers module instead of terrain in File -> Preferences -> startup.
2. Place your SC2Bank file in "Documents\StarCraft II\Banks" to use it in test mode.
3. While in test mode additional Editor cheats can be used for convenience. For full reference see [docs/SC2TestDocumentCheats.txt](docs/SC2TestDocumentCheats.txt), copy pasted from [patch 1.3.0 notes](http://us.battle.net/sc2/en/blog/2514162/patch-130-now-live-3-22-2011). Common cheats:
	* god - Turns on god mode for the selected player.
	* showmap - Toggles fog of war display and validation.
	* makeunit chain - Creates XM814 Heavy Machine Gun at cursor.
	* makeunit ammo 5 - Creates 5 ammo boxes at cursor.
	* makeunit eos 1 14 - Creates 1 Eos for player 14 at cursor.
	* deathunit - Kills the selected units.
	* move - Moves the selected units to the cursor position.
	* xp 10000 - Adds 10000 XP to the selected units.
4. Triggers can be manually run with TrigRun, however the naming may be a bit confusing. To run Sec B hades fight trigger named "STW16b - Boss Fight (Hades)" type "trigrun STW16bBossFightHades". Spaces, minus and parentheses are removed, name is case sensitive, so "trigrun stw16bbossfighthades" will not work.
5. For testing purposes it may be usefull to disable certain story/world triggers, like ambient spawns.

## Original instructions
Original instructions by ArcanePariah on [forum](http://notdstarcraft.com/threads/notd-1-repository.3631/) are copy pasted here for convenience.

1. I am presuming you know how to use Git. If not, a primer can be found here: https://git-scm.com/doc. If you need a GUI frontend for Git, I would suggest SourceTree: https://www.sourcetreeapp.com/
2. You MUST make a folder named "Night of the Dead" in your Mods folder in your Starcraft II install folder (so the full path must be Starcraft II/Mods/Night of the Dead), and clone to this folder so dependencies will be resolved correctly. You will NOT have access to the online version of the dependency.
3. I will accept pull requests on Github or patches directly on Github. Please create a bug report on this forum if one does not already exist, and then link to the patch, so I can review it.
4. Any changes to the binary SC2Map file will be discarded. I will only integrate changes to the unpacked map files.
5. Please test any changes you make locally. If you need help on this, I can provide a list of test mode cheats.
6. If I believe your changes are high risk, I will publish them to the test map first, unless I can verify it myself that it won't break anything.
7. If you do not know what a particular part of the editor does, you can find me on the SC2Mapster Discord channel: https://discord.gg/Ggww95E
