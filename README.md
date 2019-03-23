![Thumb](/Other/Graphics/banner.png)
## Xbox Softmodding Tool v1.1.6
### Created by Rocky5

###  Background:

I set out to try and make the softmodding process as pain free and user friendly as possible and to be honest I think I nailed it. You don't need to have a specific MS dashboard version or mess about in menus trying to backup your EEPROM.bin or even working out what version to install. I take all that and do it for you, I backup the EEPROM.bin I give you an easy to use settings menu ( NKPatcher Settings ) that has all the info you need to get the just of things. I have also made it as safe as I possibly can, by having recovery dashboards and fail safes in place in case you remove your dashboard or you format your E partition eg... you can always recover.
		
#### I even added support for 24 dashboard locations, so every other softmod dashboard install location is covered.

Note: Making changes in the unprotected C partition is not advised unless you know what you are doing, you will know you are in this mode if you see a folder named "Do not touch anything in here" lol

### Contributions
 If you'd like to say thanks by sending a small donation, it'd be a huge help, and it'll allow me to keep spending time towards contributing to the Xbox community in the future.

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=65NJWU9PUUX7W&lc=GB&currency_code=GBP&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHosted)

## Installation
 ### Download Prebuilt versions: [Download](https://drive.google.com/drive/folders/0BzRN8P835YijRU94cVNNWFA1Z28)
 
 #### Build from Source: (Note: this is only for advanced users)
 * Download [Xbox Softmodding Tool](https://github.com/Rocky5/Xbox-Softmodding-Tool/archive/master.zip) and extract the **Xbox-Softmodding-Tool-master** folder to your desktop.
 * Navigate to the **Xbox-Softmodding-Tool-master** directory and double click **Build Release.bat**
 * Wait till it's done doing its thing and it will then open a new window with the built source files all ready for use.
 * [Youtube - How to setup your USB Pen and install a Softmod](https://www.youtube.com/watch?v=FnL1ttepaDo)

### Main Features:

 * Supports all Xbox versions
 * Supports all currently exploitable games including the new Tony Hawks Pro Skater 4
 * Obviously runs unsigned code
 * Doesn't require a certain Microsoft Dashboard version
 * User friendly interface
 * Information buttons on all menus
 * Mandatory ShadowC partition
 * Increased ShadowC partition size (485mb)
 * Small footprint *
 * Dualbooting support
 * Simple and easy to use settings menu
 * Repair missing dashboards, right from the Xbox
 * Repair Softmod right from the Xbox
 * Extremely simple to install
 * Extremely difficult to break the softmod
 * Supports the Xbox HDD partition table
 * Built in back door if you break your dashboard. ( Hold Start+Y on startup )
 * Allows you to NULL the HDD Key
 * Allows you to switch video regions
 * Persistent Softmod Mode
 * Clock auto set to 01/01/2017 (No more clock loops)
 * Multiple dashboard locations built in
<details>
  <summary>Show dashboard locations</summary>
  
 * C:\XBMC-Emustation\default.xbe
 * E:\XBMC-Emustation\default.xbe
 * F:\XBMC-Emustation\default.xbe
 * C:\XBMC4Gamers\default.xbe
 * E:\XBMC4Gamers\default.xbe
 * F:\XBMC4Gamers\default.xbe
 * C:\XBMC4Xbox\default.xbe
 * E:\XBMC4Xbox\default.xbe
 * F:\XBMC4Xbox\default.xbe
 * C:\XBMC\default.xbe
 * E:\XBMC\default.xbe
 * F:\XBMC\default.xbe
 * C:\dashboard\default.xbe
 * E:\dashboard\default.xbe
 * F:\dashboard\default.xbe
 * C:\dash\default.xbe
 * E:\dash\default.xbe
 * F:\dash\default.xbe
 * E:\default.xbe
 * E:\dashboard.xbe
 * C:\evoxdash.xbe
 * E:\evoxdash.xbe
 * C:\XBMC.xbe
 * E:\XBMC.xbe
 
</details>

### NKPatcher Settings:

NKPatcher, this is the second stage of the Softmod. This is what patches the kernel after the NDURE exploit is executed and gives you all the lovely unsigned code and fancy features.

NKPatcher Settings allows you to modify certain aspects of NKPatcher in a safe manor.	

At the top of each menus there is an "Information" button, this will give you a description of the menu you are in.


### Dashboard Settings
  > ### Backup, Restore or Move
  * This is used to move or restore a clean copy of UnleashX, as well as backup your dashboards.
  > ### Dual Booting
  * #### Enable:
	This option is used to enabled dual booting, you get asked if you would like a dashboard setup for you when you select this option.
  * #### Disable:
	This option is used to disabled the dual booting process. You are also asked if you would like the alt dashboard to be removed.
  * #### Update:
	This option is to be used if you want to use your own custom dual booting path, you can use the "OpenDash Dualboot.settings" tool to do this, it explains things.
  * #### Restore:
	This option will restore the stock dualboot.settings file.

	
### EEPROM
  * #### Enable:
	This option will enable the virtual eeprom. This will install a copy of your Xbox eeprom.bin to the HDD and use it instead of the onboard one.
  * #### Disable:
	This option will disable the virtual eeprom. Allowing you to edit the onboard one. ( not recommended to go modifying the eeprom if you don't know what you're doing )
  * #### Backup EEPROM Tool:
	This option will load my "Xbox Softmod Tool Kit" and backup the eeprom. You will be taken back to the NKPatcher Settings when complete.
### EEPROM > Advanced Features
  > ### Hard Drive
  * #### Null Key:
	This option will allow you to NULL your eeprom Key and relock your Hard drive to this new key. This allows the creation of new hard drive's or fixing your current hard drive a doddle as you will be able to lock these drives with a 32 zero key.
  > ### Persistent Softmod
  * #### Enable:
    This option will allow you to re-enable the persistent softmod mode. What this mode does is puts the Xbox into a controlled error 16 state. Don't be alarmed!. This is 100% safe, as long as you don't remove anything from the real C partition. In this mode every game is loaded under the softmod, what this means is IGR on all retail (original) games and never needing worry about losing your softmod again, though with my softmod that's a moot point.
  * #### Disable:
    This option will allow you to disable the persistent softmod mode. In this mode your xbox will work like any other softmod out there, retail (original) games will bypass the softmod.
  > ### System Language
  * #### Select a language:
    This option will allow you to change the system language at the eeprom level, ie this will change the games ingame languages for PAL releases.
  > ### Video Region
  * #### Set Video to NTSC:
    This option will allow you to change your Xbox video region to NTSC, so you can get those lovely HD resolutions. ( using a component cable )
  * #### Set Video to PAL:
    This option will allow you to change your Xbox video region to PAL, so you can play some of the PAL exclusive games that don't work when set to NTSC.
	

### Fan speed
  * #### Self explanatory.


### Hard Drive
  > ### Partition Types
  * #### Default:
	This is the standard/default option, this allows Partition 6 ( F ) to use all available extra space.
  * #### Partition F & G:
	This option allows a F and G partition. Where F takes upto 137GB and G takes the remaining space of the drive.
  * #### XBPartitioner:
	This option is a placebo option, all above options will allow the partition table, I just added this for simplistic reasons.
  > ### Populate partitions
  * #### E Partition:
	Creates "Applications, Emulators, Games and Homebrew" folders.
  * #### F Partition:
	Creates "Applications, Emulators, Games and Homebrew" folders.
  * #### G Partition:
	Creates "Applications, Emulators, Games and Homebrew" folders.


### Kernel Fonts
  * #### Displays current font used for the NDURE exploit.
  * #### Advanced Features.
### Kernel Fonts > Advanced Features
  > ### Backup Xbox Bios
  * Backs up the Xbox Bios to E:\Backups\Bios
  > ### Kernel Font Options
  * #### Install Kernel Font:
	This option will install a kernel specific font. This isn't really needed but if there are boot issues this can fix the issue.	
  * #### Restore Generic Font:
	This option will restore the generic font to the Xbox. This font works on all Xbox kernel versions and is the default font used.
  > ### XTF Font Delay Options
  * #### Remove all:
	Removes these delay files.
  * #### Install 1 Delay file:
	Installs 1 delay file, in hope it fixes your boot issue.
  * #### Install 2 Delay files:
	Installs 2 delay file, in hope it fixes your boot issue.
  * #### Install 3 Delay files:
	Installs 3 delay file, in hope it fixes your boot issue.
  * #### Install 4 Delay files:
	Installs 4 delay file, in hope it fixes your boot issue.
  * #### Install 5 Delay files:
	Installs 5 delay file, in hope it fixes your boot issue.


### LED colour
  * #### Self explanatory.


### Video modes
  * #### Default:
	This is the default mode, supports all video mode.
  * #### Force Progressive:
	This option will force 480p video mode even if your game doest support it. Note: This will make the image distorted in PAL video mode.
  * #### Force VGA:
	This option will force VGA video mode. Note: This requires a compatible monitor that support sync on green, also it may not work on v1.6 Xbox properly.
  * #### Flicker Filter:
	Used to change the blur amount when using 480i and 576i video signals.


### Modules & Settings
  > ### Modules
  * #### Built in Modules
	These are what I use to do specific tasks.
  * #### User Modules
	If you make your own, you will see them here. ( you add your own to the modules folder inside the NKPatcher Settings App )
  > ### UnleashX Settings
  * #### This is the settings menu for UnleashX, change network settings video settings eg...



### Xbox Softmodding Tool Extras Disc:

		
 * #### Install alternative dashboards
    * Avalaunch
    * EvolutionX
    * UIX Dash
    * UnleashX
    * XBMC 3.5.3
    * XBMC4Gamers
    * XBMC-Emustation
			
 * #### Install useful applications
    * DVD2Xbox
    * DVDX v2
    * EEPROM Backup Tool
    * Enigmah-X
    * NKPatcher Settings
    * Xored Mini launcher with 882 trainers
    * Note Alt Dashboards can be installed as applications.
			
 * #### Install game mods & homebrew  (Note not included in the GitHub build as it was to large.)
	#### -- Homebrew --
    * Aliens versus Predator Gold
    * DoomX
    * Super Mario War 1.8
    * Super Mario War 1.8 Halloween Edition
    * xDuke
	#### -- Mods -- (only on prebuilt version)
    * FIFA 07 - real gameplay mod
    * Operation Flashpoint Elite - Addons
    * Richard Burns Rally - Textures & realistic damage & physics.
    * WWE Wrestlemania XXI - CrazyChris ModPack v1, crap-loads of changes.
			
 * #### Install Microsoft dashboards
    * Official 5960
    * My hacked 4920 version
			
 * #### Clear the Xbox Cache
    * This will clear the E:\Cache folder and the X, Y & Z partitions.
		
 * #### Upgrade the 2014 Softmod to my Xbox Softmodding Tool
    * Used to upgrade from my 2014 Softmod.
			
 * #### Update the Xbox Softmodding Tool
    * This is used to update to a newer version of the softmod. Your dashboards are not touched, I only update the backend.
		
 * #### Upgrade Older Softmods to my Xbox Softmodding Tool	
    * Used to upgrade from any other softmod to mine, or install a clean softmod.
		
 * #### Restore your Xbox to an un-softmodded state
    * I install all softmod saves and the UDDAE exploit so you can resoftmod without the need for a exploitable game.
		
 * #### Advanced Apps
    * Chimp 261812
    * ConfigMagic v1.6.1
    * XBPartitioner
    * XBP Table Writer
		
#### As well loads of other features.			



### Update, Upgrade & Restore info:

#### Updating the Xbox Softmodding Tool to the latest version:
 You can use the "Xbox Softmodding Tool Extras Disc" to update the Softmod.
 All you need to do is burn the new ISO & select the "Update Xbox Softmodding Tool" option, located in the "Advanced Features" menu, just follow the on-screen instructions.

#### Updating the 2014 Softmod to the Xbox Softmodding Tool:
 You can use the "Xbox Softmodding Tool Extras Disc" to update the Softmod.
 All you need to do is burn the new ISO & select the "Update 2014 Softmod" option, located in the "Advanced Features" menu, just follow the on-screen instructions.

#### Upgrade Older Softmods:
 You can use the "Xbox Softmodding Tool Extras Disc" to update older Softmods to my new softmod.
 All you need to do is burn the new ISO & select the "Upgrade Old Softmods" option, located in the "Advanced Features" menu, just follow the on-screen instructions.

#### Restoring to a clean install of my Xbox Softmodding Tool:
 You can use the "Xbox Softmodding Tool Extras Disc" to install a clean install of my Xbox Softmodding Tool.
 All you need to do is burn the new ISO & select the "Upgrade Old Softmods" option, located in the "Advanced Features" menu, just follow the on-screen instructions.

#### The great thing about the above, is it requires no FTP access or knowledge on how to update/restore softmods, great for people who are new to the Xbox scene.



### Source code:

 This softmod is fully open source, you can find the full source code on my GitHub with everything I have used/created in a nice organised manner.
 If you are a windows user, I have created batch files to do most of the heavy lifting, so it makes my life and yours simple when building stuff.

 * **Note:** The Xbox XDK and Microsoft Visual Studio .NET 2003 is required to build some of the tools.
   * [GitHub](https://github.com/Rocky5/2016-Softmodding-Tool)


### [Youtube Channel](https://www.youtube.com/JCRocky5):
 There you can find videos on "How to setup your USB Pen and install a Softmod", "How to clone your Hard drive using Chimp 261812 from start to finish." and many other crappy videos I make for the Xbox.


### Acknowledgments:

I would like to thank the following, without there contributions to the Xbox scene we would not have what we have today.

#### Original NKPatcher:
 Rmenhal without this guy we wouldn't have NKP or the advanced fonts we use today.
#### NKPatcher Unofficial Edits:
 Xman954 & kingroach added some cracking features to NKPatcher.
#### PBLoader - Metoo Edition:
 Team Phoenix, ldotsfan, & Rmenhal
#### Configmagic source code:
 Team Assembly & Yoshihiro
#### UnleashX:
 James for such an amazing dashboard, without his work on UnleashX there would be no Softmod installers as we know it.
#### The original XBMC team
 For XBMC Shortcut XBE Source
#### MS Source leak:
 & without this person we wouldn't have the bios files or NKPatchers we have today.
#### Background Music
 http://www.looperman.com/users/profile/1795296 - vibes piano 3
#### New TH4 save game exploit:
 Grimdoomer ( thefallen93 )
#### To all the tester that helped me squash bugs and improve features & to anyone else I may have forgot.
