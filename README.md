# Fixed Launchers for Command & Conquer: The Ultimate Collection

<p align="center">
 <a href="https://www.moddb.com/games/cc-generals/downloads/new-fixed-ultimate-collection-launchers-v101" title="Download *New* Fixed Ultimate Collection Launchers v1.01 - Mod DB" target="_blank">
  <img src="https://button.moddb.com/download/medium/197063.png" alt="*New* Fixed Ultimate Collection Launchers v1.01" width=390 height=75 />
 </a>
</p>

<p align="center">
 <a href="https://github.com/Medstar117/CNC-Ultimate-Collection-Fixed-Launchers/blob/master/Patch%20Notes.txt">
  <span>
   <strong>>>>>>>>>>LATEST PATCH NOTES<<<<<<<<<</strong>
  </span>
 </a>
</p>

Author:	Medstar

Discord:	@Medstar#1550

Donate: <a href="https://www.paypal.me/chancegregurek">PayPal</a>

## Description
This installer includes my custom fixed launchers for Command & Conquer: The Ultimate Collection. These fixed launchers re-enable command-line parameters to pass through to your games; and this installer will also add in some missing registry keys that re-enable the ability to use custom maps. These launchers also make it to where you can launch directly from the games’ respectful game exe’s (e.g. CNC3.exe)--completely bypassing the launchers entirely.

Hope y'all enjoy :D

## Disclaimer
These launchers aim to **emulate** the now-publicly-unavailable fixed launchers from Bibber. I have re-created the launchers from scratch using AutoIT; they **ARE NOT** the same launchers that Bibber made. The source code used to compile these launchers and the installer **ARE NOT** the same as Bibber’s; therefore, **NOTHING IN THIS INSTALLER IS COPYRIGHTED BY BIBBER**. I made sure of that as to avoid any possible copyright stuff with him. I don't want to mess with any of that crap; I respect him for his work, and I respect his decision in taking down his launchers. I just want to make my stuff work how ***I*** want it to work, I want my games to work how ***I*** want them to work (in that I want them to work as ***they should have from the get-go)***, and I want to share my stuff with the community since it all works great for me.

**TLDR:** The launchers themselves are of my own work (as you can see in the details of the exes’ properties); everything else is owned by their respectful owners (e.g. the No-CD patched exe’s, any community patches included in this installer, any artwork used in the installer wizard, the games themselves, etc). Bibber is the OG that inspired me to make my own launchers for the community to try out. These launchers are ***similar*** to Bibber's--they are **NOT** direct copies of his, since that would infringe on his copyright (of which I respect).

Finally, use these launchers at your own risk; and I hope they help you out as much as they've helped me out.

# IMPORTANT NOTES
***PLEASE*** disable "Origin In Game" and the "Cloud Saves" feature for each game prior to using the installer. Doing so will save you a lot of headaches and incompatibilities. The "Origin In Game" feature most notably will overwrite the fixed launchers for your games when you try to launch them--it's like a pre-launch check of the game files. You can disable them by right clicking your game in your Game Library in the Origin desktop app, selecting Game Properties, then unchecking the boxes for each feature.

# Features
The installer features a game selection page where one selects the game they want to add the new launchers to. The installer then replaces the following:
  1) The original game launcher exe with one that I've made with AutoIT
  2) Any necessary game exe's with No-CD patched versions (only applies to games prior to C&C3; those exe's are directly patched to not have command line functionality at all)
  3) All associated .par files with ones patched to not require Origin to launch when launching a game (be mindful that Origin still has to be installed for the games to actually work; this more or less prevents it from launching ALONGSIDE the game as well as preventing Origin from overwriting my fixed launchers)
  
**If you want any other features included in this installer, feel free to add an issue and label it with the "feature request" label.**
  
  ### **For C&C95**
The 1.06c patch made by Nyerguds is also installed as a necessary feature. Permission has been granted to me to use this patch by Nyerguds within my installer. The patch includes bugfixes and other features to enhance the overall gameplay of C&C95 along with making the game properly compatible on most modern machines. More info available here concerning the 1.06c patch:

http://nyerguds.arsaneus-design.com/cnc95upd/cc95p106/patch106c_r3_en.html

  Thank you again, Nyerguds, for allowing me to include your patch in this launcher.

  ### **For Generals/Zero Hour**
  Since this is a recurring issue with both games, the installer automatically removes "dbghelp.dll" from both game directories as to avoid the on-launch-crash that occurs (Technical Difficulties, Serious Error, etc).
  
  Another recurring issue is the game crashing on launch due to the "options.ini" file. The file itself could be either missing from one's Documents folder, or it could have the incorrect resolution set for the game. I've made a tool called "ResEdit" (aka, "Resolution Editor") that automatically either edits these files with the correct resolution information, or it automatically makes one with the proper resolution set in case the file is missing entirely.
  
  ### **For TW/KW, RA3/Uprising, and Generals/Zero Hour**
  Another recurring issue is the fact that one can't use custom maps right on download with these five games. The installer adds in the needed registry key for these games to recognize custom maps.

# Command-Line Parameters Exclusive to The Launchers

### This applies only to “Generals.exe”, “CNC3Launcher.exe”, “RA2Launcher.exe”, and “RA3Launcher.exe”.
- -game gen|genep1|cnc3|cnc3ep1|ra2|ra2ep1|ra3|ra3ep1
  - Launches the game directly instead of popping up the window for choosing.
    - cnc3		    = C&C 3: Tiberium Wars
    - cnc3ep1	  = C&C 3: Kane's Wrath
    - gen		     = C&C: Generals
    - genep1	   = C&C: Generals: Zero Hour
    - ra2		     = C&C: Red Alert 2
    - ra2ep1		  = C&C: Red Alert 2: Yuri's Revenge
    - ra3		     = C&C: Red Alert 3
    - ra3ep1		  = C&C: Red Alert 3: Uprising

### **Example:**
- To launch Kane’s Wrath directly, and to launch the Game Browser interface for it, I would use this in either the Target field in a shortcut or as a command in the Command Prompt:

  - “C:\Users\Medstar\Origin Games\Command and Conquer 3 TW and KW\CNC3Launcher.exe” -game cnc3ep1 -ui

- In the Origin desktop app, I would put this in Game Properties > Advanced Launch Options for Tiberium Wars/Kane’s Wath:
  - -game cnc3ep1 -ui

# Uninstall
In the Origin desktop app, right-click your games’ portraits and select the “Repair” option.
