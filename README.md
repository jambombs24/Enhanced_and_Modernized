# Enhanced and Modernized
Github page for the Skyrim load order Enhanced and Modernized.

The list itself is here: [Skyrim 2023 Mega Mod List](https://www.nexusmods.com/skyrimspecialedition/mods/82863).

The Wabbajack files are here: [Enhanced and Modernized - Wabbajack Modlist](https://www.nexusmods.com/skyrimspecialedition/mods/93277).

## Requirements

- Skyrim AE in your Steam library, WITH the Anniversary Edition upgrade.
- 160GB of free space, which must be on one drive (139 for installation, 20 for page file, and then 1 more for whatever else generates.
  - At least 200GB is recommended, so you can make an even larger page file, or store extra files.
  - This drive must have at least 15% of completely free space left over.
- Another 82GB for mod downloads, on any drive (installation speed is as fast as the slowest drive).

## Installation Guide

### Step One: Prepare Your Computer
To help make the game run as well as possible, you need to increase the size of the page file.

- Start typing "Advanced system settings" into your Windows search bar, and select "View Advanced System Settings" when it appears.
- Switch to the Advanced tab.
- Press the Settings button in the performance section.
- Switch to the Advanced tab (again).
- Press the Change button in the "Virtual memory" section.
- Uncheck the box that auto-manages page file size.
- Select whatever drive you plan to install Skyrim on.
- Select the "Custom size" option.
- Set the minimum to at least 20480 (20GB), and the maximum to something higher (recommended: 40960 (40GB)).
  - Note: You need to have enough free space on your drive to fit the whole page file.
- Press "Set" to commit your changes.
- Keep pressing OK until you get out of all the settings windows.
- Restart your computer.

### Step Two: Prepare Skyrim
Uninstall Skyrim completely from your system. Then delete the whole Steam directory, which is typically something like *~\Steam\steamapps\common\Skyrim Special Edition*. Also delete the Skyrim folder at *~\Documents\My Games*.

Now we're going to reinstall it! Install the game.

After doing this, you should have a **completely unmodified Skyrim installation**.

Now launch Skyrim through Steam. Let the launcher set a graphics preset, and then load to Skyrim's main menu. You should get the popup to download the Anniversary Edition Creation Club content. Go ahead and download all those. Once all the creations are downloaded, exit Skyrim entirely.

At this point you should have a stock installation of Skyrim AE.
Let's move on.

### Step Three: Accounts
Create an account for the following websites if you don't already have one:
- [Nexus Mods](https://www.nexusmods.com/)
- [LoversLab](https://www.loverslab.com/)

### Step Four: Acquire Wabbajack
Go to [Wabbajack.org](https://www.wabbajack.org/) and download the program.

Place the downloaded executable somewhere outside of any protected files. I have it placed in *C:\Modding\Wabbajack*. When you run this Wabbajack executable, is will automatically download the latest version of the entire Wabbajack program.

Once you've launched Wabbajack, click the settings button in the top right. Connect to your LoversLab and Nexus accounts.

### Step Five: Prepare the Enhanced and Modernized installer.
Download the .wabbajack file from its [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/93277) page.

Before actually using this file, we need to prepare for where the modlist is going to go.
Create an empty directory, also outside of any protected folders, for where everything will be installed. For example, *C:\Games\Skyrim_EnhancedAndModernized*.

Open up Wabbajack if you closed it. Press the "Install from Disk" button. There are three options that must be configured:
- Target Modlist: Set this to the Enhanced and Modernized .wabbajack file.
- Modlist Installation Location: Point this to where you decided the installed modlist will go.
- Resource Download Location: This is where all the mod archives will be downloaded to. This could be anywhere, but make sure you have enough space!

### Step Six: Modlist Installation
Click the play button to the right of the config options to begin installation. This process will take some time.

Mods that are not hosted on Nexus will be downloaded first. For each of these, a browser will open with a prompt at the top of the screen telling you which file to download.

As for the Nexus-hosted mods themselves, you'll be taken directly to the exact file download you need. If you have a premium Nexus account, then you don't need to do anything else. If you have a free Nexus account, then the slow downloaded button must be clicked for each mod.

After every mod is downloaded, Wabbajack will install them all, alongside Mod Organizer 2 itself. After the installation has been completed, run MO2 to access the modlist.

In the event that the installation fails, your computer shuts off, or whatever else, you won't have to re-download any mods.

### Step Seven: Finishing Setup
The last setup task left is to install ENB.
First, download ENB version 0.493 (or newer) from the [ENB website](http://enbdev.com/download_mod_tesskyrimse.html).

Once you have the ENB .zip file, delete the enbseries_sdk archive from inside of the parent archive. You can do this by either extracting the whole zip, deleting enbseries_sdk.zip, and recompressing the rest, or by using a tool like PeaZip that allows direct archive editing.

![ENB archive folder structure.](/enb_zip.PNG)

Now drag the ENB archive into MO2's downloads area. Double-click to install. Right click on data at the top and choose to create a directory. Name it "Root" (no quotes, but make sure the R is capitalized!). Now expand the "Wrapper Version" directory, find d3d11.dll and d3dcompiler_46e.dll and drag them into Root.

After that, uncheck the boxes for Linux Version, Wrapper Version, and the two .url files.

![ENB installation heirarchy.](enb_dirs.PNG)

Press OK to install. MO2 will show a warning; install anyway. Then move the newly installed ENB mod to the top of the ENB section. You can change the name and version to the correct values if you want to.

![ENB in position.](enb_placed.PNG)

To ensure that you've done this correctly, you can check MO2's virtual file system. Use the explorer virtual system in the executables menu to open Explorer++, and then go up one directory. You should see d3d11.dll and d3dcompiler_46e.dll in Skyrim's root folder.

![ENB in VFS.](enb_virt.PNG)

### Step Eight: Voicing

At the end of the list in MO2's left panel, you'll see a section labaled optional. This is where the Dragonborn Voice Over mod and related content have been placed. I've placed these here because some people like having their character voiced, and others prefer their character to remain unvoiced.
  
If you do not want your player character to have voiced lines, disable all of these mods. If you do want the player character to speak, then leave these enabled.
  
Also, if you're using some kind of surround sound, enable "Dragonborn Voice Over - Surround Plugin Replacer" and "Dragonborn Voice Over - Reverb Interior Sound Expansion Patch - Surround" to make sure audio plays properly.
  
### Step Nine: Skyrim

Read [this article](https://www.nexusmods.com/skyrimspecialedition/articles/5316).

Then you're free. Go play the game.
