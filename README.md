# Superwow Installation Guide
<hr>

![image](https://github.com/pepopo978/SuperwowInstallation/assets/149287158/833d8d7e-c0c9-456a-9886-dc913ec07bfa)
### 1.  Disable windows real time protection (it will turn back on automatically after a short time) as it will block downloading vanillafixes and superwow.  
<hr>

![image](https://github.com/pepopo978/SuperwowInstallation/assets/149287158/4e54f864-445b-4fb8-a8f6-f1c58eb53fc1)
### 2.  While you have windows security open, add a folder exclusion for your base turtle wow folder (where WoW.exe is) so that it doesn't remove vanillafixes/superwow later on out of nowhere.
<hr>

### 3A. If you plan on using the TWOW launcher:
#### 1. Go to the addons tab and add Superapi
#### 2. Skip to [step 6](https://github.com/pepopo978/SuperwowInstallation?tab=readme-ov-file#6--download-the-latest-superwow-dll-from-here-httpsgithubcombalakethelocksuperwowreleasestagrelease-and-place-in-your-twow-folder-next-to-wowexe--you-only-need-the-dll-you-dont-need-the-launcher) 
<br/>

### 3B.  Otherwise: Download the latest vanilla fixes (>= version 1.4) if you don't already have it from here https://github.com/hannesmann/vanillafixes/releases and place in your TWow folder next to WoW.exe.  
You may need to add `d3d9.enableDialogMode = True` to your dxvk.conf file if you are getting black screens when alt-tabbing or switching windows.
<hr>

### 4.  (Optional) If you want VanillaTweaks as well:
- Download tweaks here https://github.com/brndd/vanilla-tweaks?tab=readme-ov-file#current-patches and place in your TWow folder next to WoW.exe
- Copy + paste `WoW.exe` so you have a backup of it
- Drag `WoW.exe` on top of `vanilla_tweaks.exe` or run `./vanilla-tweaks WoW.exe` from the command line in the directory containing `WoW.exe` and `vanilla-tweaks.exe`.  If you want to specify specific options like increasing nameplate range you have to use the command line.  See https://github.com/brndd/vanilla-tweaks?tab=readme-ov-file#usage for examples
- Rename either `WoW_tweaked` to `WoW` or `WoW_tweaked.exe` to `WoW.exe` depending on whether you have "Show file extensions" turned on in Windows.  Be careful not to accidentally make the filename `WoW.exe.exe` if you don't have "Show file extensions" turned on in windows.
<hr>

### 5.  Download the latest SuperWoW api addon from here https://github.com/balakethelock/SuperAPI and place in Interface/Addons making sure to remove the "-master" suffix appended by github.  
In the minimap icon this adds you can configure the behavior for the following:
- autoloot
- clickthrough
- background sound
- sound cap
- fov
- selection style
<hr>

### 6.  Download the latest SuperWoW dll from here https://github.com/balakethelock/SuperWoW/releases/tag/Release and place in your TWow folder next to WoW.exe.  You only need the dll you don't need the launcher.
<hr>

### 7.  Make sure SuperWoWhook.dll is in your dlls.txt file.  This file is located in your TWow folder next to WoW.exe.  
If you are using vanillafixes it should already be there, if using the TWOW launcher you'll need to add it yourself.  The order doesn't matter, here's an example of the contents of my dlls.txt:

![image](https://github.com/user-attachments/assets/09e5e5fb-657e-42a0-968a-24920bf27e14)

<hr>

### 8.  (Optional) If you want to see improved enemy castbars pick ONE of these options:
<b>Don't use both of these together.</b>
#### Option 1 PFUI
Download the latest PFUI from here https://github.com/shagu/pfUI and place in Interface/Addons making sure to remove the "-master" suffix appended by github.
#### Option 2 SuperAPI_Castlib
Download the latest SuperWoW castlib addon from here https://github.com/balakethelock/SuperAPI_Castlib and place in Interface/Addons making sure to remove the "-master" suffix appended by github.
<hr>

### 9.  If using the TWOW launcher use that to start the game.  Otherwise launch VanillaFixes.exe to start the game.  The first time it should pop up a dialog saying which dlls it is loading and SuperWoW should be one of them.
<hr>

### 10.  In game open up a macro and if you have 512 allowed characters Superwow is working
<hr>

### 11.  (Optional) Ignore this if already did this when installing SuperAPI.  If you were using vanillatweaks for sounds while the game is in the background, run `/run SetCVar("BackgroundSound", "1")` to reenable that.  Can also do `/run SetCVar("UncapSounds", "1");SetCVar("SoundMaxHardwareChannels", "64");SetCVar("SoundSoftwareChannels", "64");` to enable the game to play more simultaneous sounds.
 
Can view other CVars and features provided here https://github.com/balakethelock/SuperWoW/wiki/Features

### 12. If you are getting either of these errors launching
![image](https://github.com/user-attachments/assets/00807ba1-53a3-4485-be76-a83c866bc48b)
![image](https://github.com/user-attachments/assets/a017feb5-87d9-429e-9252-156554ecd113)

On Windows: Go to Control Panel > System and Security > System > Advanced system settings. Under Performance, click Settings, then the Data Execution Prevention tab.

Select Turn on DEP for all programs and services except those I select, and add WoW.exe to the list. (Remember to remove this later if it doesn’t help you.)

This can also be caused by not having any Visual c++ redistributables installed, try installing using this link:

32 bit x86: https://aka.ms/vs/17/release/vc_redist.x86.exe (probably just need this one)

64 bit x64:https://aka.ms/vs/17/release/vc_redist.x64.exe
