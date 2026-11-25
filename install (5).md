---
layout: modlist
modlist: everwild
title: Everwild: Install
---

# Installing Everwild

Follow these steps in order. A clean install of Skyrim avoids most problems.

## How to clean install

### Step 1: Uninstall via Steam

1. Open your Steam Library.
2. Right-click The Elder Scrolls V: Skyrim (or Special Edition), hover over **Manage**, and click **Uninstall**.

### Step 2: Delete residual game and mod folders

Even after uninstalling through Steam, leftover files and mod configurations remain and can cause bugs. Manually delete the following:

- **Steam game folder:** Navigate to `..\Steam\steamapps\common` and delete the Skyrim or Skyrim Special Edition folder.
- **Documents folder:** Navigate to `C:\Users\[Your User Account]\Documents\My Games` and delete the Skyrim or Skyrim Special Edition folder.
- **Local AppData:** Press Windows Key + R, type `appdata`, hit Enter, open the **Local** folder, and delete the Skyrim or Skyrim Special Edition folder.
- **Mod managers:** Delete any leftover mod manager folders (such as Vortex or Mod Organizer 2) in your AppData directories if you are resetting your setup.

### Step 3: Reinstall the game

1. Go back to your Steam Library and click **Install** on Skyrim.
2. Avoid installing the game into the `C:\Program Files` or `C:\Program Files (x86)` directories, to prevent Windows permission issues with mods.
3. Launch the game once from Steam to let it generate fresh configuration files, then download all owned Creations, then close it.

## How to configure the page file

To improve system stability (especially if you have only 16 GB of RAM), set up the page file for the drive you are running Everwild on.

1. Press the Windows key and **R** together, type `sysdm.cpl`, and click **OK**.
2. Select the **Advanced** tab, and under Performance click **Settings**.
3. Select the **Advanced** tab again and click **Change**.
4. Uncheck **Automatically manage paging file size for all drives**.
5. Select the drive where Everwild is installed and click **Custom size**.
6. Set the page file size from **20000** minimum to **40000** maximum and click **Set**.
7. Click **OK**. A reboot will be required.

Don't forget that the size you set will be taken as used space on your drive.

## How to install

1. Launch **Wabbajack**.
2. Navigate to **Browse Modlists**, then select Skyrim from the list of games.
3. Locate **Everwild**, click on it, and hit **Download**.
4. Set the location for the install. Downloads should auto-fill. Hit **Install**.
5. When it has finished, launch MO2 from the folder you specified. (Optionally, right-click it and choose Send to Desktop for a shortcut.)
6. Make sure **Everwild** is selected in the drop-down and hit **Play**.

## Next steps

- Read the [Getting Started guide]({{ '/everwild/getting-started/' | relative_url }}) before your first session.
- Using the SkyrimNet profile? See the [SkyrimNet setup]({{ '/everwild/skyrimnet/' | relative_url }}).
- Need help? Join the [Discord](https://discord.gg/3UaP8ssBSv).
