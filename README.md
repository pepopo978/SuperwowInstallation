# Superwow Installation Guide
![image](https://github.com/pepopo978/SuperwowInstallation/assets/149287158/833d8d7e-c0c9-456a-9886-dc913ec07bfa)
### 1.  Disable windows real time protection (it will turn back on automatically after a short time) as it will block downloading vanillafixes and superwow.  
<hr>

![image](https://github.com/pepopo978/SuperwowInstallation/assets/149287158/4e54f864-445b-4fb8-a8f6-f1c58eb53fc1)
### 2.  While you have windows security open, add a folder exclusion for your base turtle wow folder (where WoW.exe is) so that it doesn't remove vanillafixes/superwow later on out of nowhere.
<hr>

### 3.  Download the latest vanilla fixes (>= version 1.4) if you don't already have it from here https://github.com/hannesmann/vanillafixes/releases and place in your TWow folder next to WoW.exe.  You may need to add `d3d9.enableDialogMode = True` to your dxvf.conf file if you are getting black screens when alt-tabbing or switching windows.
<hr>

### 4.  Download the latest SuperWoW dll from here https://github.com/balakethelock/SuperWoW/releases/tag/Release and place in your TWow folder next to WoW.exe.  You only need the dll you don't need the launcher.
<hr>

### 5.  Download the latest SuperWoW api addon from here https://github.com/balakethelock/SuperAPI and place in Interface/Addons making sure to remove the "-master" suffix appended by github.
<hr>

### 6.  (Optional) If you want to see improved enemy castbars:
- download the latest PFUI from here https://github.com/shagu/pfUI and place in Interface/Addons making sure to remove the "-master" suffix appended by github.
- download the latest SuperWoW castlib addon from here https://github.com/balakethelock/SuperAPI_Castlib and place in Interface/Addons making sure to remove the "-master" suffix appended by github.
<hr>

### 7.  Launch VanillaFixes.exe to start the game.  The first time it should pop up a dialog saying which dlls it is loading and SuperWoW should be one of them.
<hr>

### 8.  In game open up a macro and if you have 512 allowed characters Superwow is working
<hr>

### 9.  (Optional) If you were using vanillatweaks for sounds while the game is in the background, run `/run SetCVar("BackgroundSound", "1")` to reenable that.  Can also do `/run SetCVar("UncapSounds", "1");SetCVar("SoundMaxHardwareChannels", "64");SetCVar("SoundSoftwareChannels", "64");` to enable the game to play more simultaneous sounds.
 
Can view other CVars and features provided here https://github.com/balakethelock/SuperWoW/wiki/Features
