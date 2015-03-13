Abandoned Ship Spawner v83
EgoSoft Forum Member : corbinbird
Game : X3TC v3.2
Date : 04/18/2013

Purpose :

I got tired of the same wrecks at the same locations with the same equipment in every game start.

What It Does :

1. Creates a whole new set of wrecks to find in a new game start. RANDOM ships / RANDOM locations. Gets rid of the old/built-in wrecks.

2. At regular intervals it creates a new RANDOM wreck at a RANDOM location for the player to salvage. The trick is finding it.

3. All wrecks have randomized equipment left onboard.

4. Auto cleanup of excessive numbers of unclaimed wrecks.

VERY IMPORTANT : (Install Instructions)
First activate the script editor. Won't work/start otherwise. For setup to complete in the game, you must dock, save, exit to the main menu and reload. Just like activating the script editor.

For X3TC v2.5 or Previous : The AL plugin is set to do the heavy work on the second reload. Nasty setup crash otherwise.
For X3TC v2.7.0 or Later : the AL plugin engine has been modified. reinit script cache not recommended. the AL plugin engine ignores the control state array. dock, save, exit and reload for setup to complete.

NOTE :
it really is RANDOM. So is the cleanup.
Tested in Custom Game/X Universe.
Abandoned ships limited at 20 max. (Conserves CPU resources.)
Turrets on spawned ship set to [None](None.md). (Conserves CPU resources.)
Debug output commented out.
AL plugin is installed Off / Disabled
All ships are possible wrecks.

Required :
None.

Recommended :
Cycrow's SatelliteEarlyWarningSystem is very helpful at detection.

Compatability :
tested with 'NPCBailAddon' & 'SalvageCommandsandNPCs'.
'SalvageCommandsandNPCs' do not salvage these spawned ships.
'NPCBailAddon'-> your choice
'Find Free Ships'-> good cheat script :)
Not tested with any [MOD](MOD.md)/.XSP that adds ships. added ships will NOT be spawned.

TO DO :
(Done->) Fix the turret cmds to 'None' on spawned ships if possible.
(Done->) Randomize the wares on wrecks that have some.
(Done->) Have cleanup cleanup more than one wreck at a time if necessary.
(Done->) get rid of the standard wrecks in every game start. Already have test script.
(Done->) Replace the 19 or 20 standard wrecks with a random 19 or 20 wrecks (random locations too) at new game start.

Changes :
lib scripts using global variable/arrays
global variable/array format tested, retested. Setup/Run only once.
improved debug output. Commented out for release.
Setup script built. Lowers CPU load after initail setup.
t file conflict solved
(v69) AL Event Handler restructured, finally understood 'Arguments'. for AL plugin they set TaskID and Script Priority.
(v70) Figured out how to have the setup set the turret defaults for {Neutral Race}. Have fixed the turret cmd settings on spawns. AL Setup script.
(v71) Minor cosmetic changes. Uninstall reworked.
(v73) bulk cleanup, bulk spawn, and lib setup scripted/completed. some testing. bulk ops now set for second load (setup crash otherwise.) AL Event Handler also got some love.
(v76) randomized wares on ALL spawned ships. no striped ships anymore.
(v77) updated read me. repackaged.
(v78) typos fixed. 'On Stack' pileup debugging started. Updated for X3TC V2.7.1
(v79) 'On Stack' problem resolved. the 'jump out of existance' command was guilty.
(v80) ware randomizer improved. does cargo/rudder/engine. M8 get some missiles. debug commented out.
(v81) minor correction to scripts. Investigated reported cargo problems. Not due to these scripts.
(v82) minor tweak to AL Event handler script. Included a non-SPK package in the download.
(v83) kill undocumented kill timer ( flying ware type timer. ) on SE Create Ship Command. Adjust global vars. Renamed/replaced lib scripts.

Special Thanks To :
'LV' for Examples and Tutorials (X3TC BountyBoost)
'Cycrow' for Examples and the script structure. (X3R BBS Extras)
'Apricotslice' for Examples and Concept. (X3TC Create Abandoned Ships on Startup)
'MarCon' for MSCI info.
'Nafensoriel' for On Stack problem notification.

No Wares/No Custom Wares Used.
No Command Slot/ID's Used.

Package Type :
AL plugin

t file  :
7300-L044.xml

scripts :
al.plugin.A.S.S.xml
al.A.S.S.event.xml
plugin.A.S.S.cleanup.xml
plugin.A.S.S.setup
plugin.A.S.S.spawner.xml
plugin.A.S.S.bulk.cleanup.xml
plugin.A.S.S.bulk.spawn.xml
plugin.A.S.S.setup.lib.xml
plugin.A.S.S.wares.xml
lib.A.S.S.random.m0.xml
lib.A.S.S.random.m1.xml
lib.A.S.S.random.m2.xml
lib.A.S.S.random.m3.xml
lib.A.S.S.random.m3p.xml
lib.A.S.S.random.m4.xml
lib.A.S.S.random.m5.xml
lib.A.S.S.random.m6.xml
lib.A.S.S.random.m7.xml
lib.A.S.S.random.m8.xml
lib.A.S.S.random.tl.xml
lib.A.S.S.random.tm.xml
lib.A.S.S.random.tp.xml
lib.A.S.S.random.ts.xml

uninstall script :
uninstall.ASS.xml

Permissions :
I consider this package community property / public domain.
If you can think of it ... go for it.
You have my permission.

EgoSoft Forum Member : corbinbird