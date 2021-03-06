No One Lives Forever Modernizer (v1.006 Modern)
-----------------------------------------------
https://heythere.coffee/nolf/

The goal of NOLF Modernizer is to help fix some long standing bugs, and update some more outdated features of the game.

-- How To Install

Place all the files in your No One Lives Forever game directory. 
Then launch NOLF.exe, and click "Advanced", and then "Customize". 
Simply "Add" the Modernizer.rez file, and check "Always load these rez files", then click "Ok", and launch the game!

It's important that you don't run this mod with any other mods that may have modified the game code. 

-- Features

 - Working multiplayer out of the box
 - Cap framerate during menus and gameplay to 60fps
 - Fixed the mouse stutter
 - Optimized performance in select cases
 - Jukebox to play some of your favourite in-game tunes
 - Supports the Game of the Year edition

-- Patch 1

 - Fixed a bug with defusing bombs and activating some switches.

-- Patch 2

 - Added 'NoRawInput' to disable mouse raw input.
 - Fixed missing continue button on mission summary screen.
 - Improved loading screen time (...that I broke, oops!)
 - Fixed some invisible impassible geometry.
 - Added a experimental developer console, can be toggled on/off with tilde. (`~`)
 - Fixed a crash in the weapons hotkey screen.

-- Patch 3

 - Bumped version to 1.006.
 - Patched out GameSpy from dedicated/hosted servers and the server browser.
 - Fixed a bug in ai path finding causing values to not always be accurate.
 - Fixed a silent out of range bug that could cause enemies to disappear and travel to a nearby galaxy at FTL speed!
 - Made the console key rebindable. (It's at the very bottom of the custom controls list.)
 - Added Big Head Mode! It's currently a little buggy, but humourous. Check the console command list on how to enable it.
 - Included some patched binaries to help improve compatibility. 
 - Added a windowed mode toggle to the display options.
 - Added anisotropic filtering to advanced performance options.
 - Fixed shadows disappearing between cutscenes and saved games.
 - Added a "Blackscreen Fix" work around for Intel HD graphics chips in Display options.

-- Important For Intel HD Graphics Users
Please enable "Intel HD Graphics Fix" in Display options. This fixes the blackscreen while underwater bug. It also switches to an alternate rendering of screen tinting, that should fix missing screen effects.

--  Control Changes
We've made some changes to the default control scheme in 1.006 Patch 3. As such the game will reset your controls on startup.

 - Scroll Wheel Up/Down     - Now handles switching weapons instead of handling scope zooming.
 - Middle Mouse/Mouse 3     - Now handles toggling between scope zoom modes.
 - `/~                      - Now toggles the console on or off.

--  Additional Config/Console Commands

We've added new autoexec.cfg commands! (They also work in the console!)

Some of these will show up in your autoexec.cfg as you set them, but if it's missing you can simply add it yourself.

"FramerateLock"			    - Locks the framerate if the value is 1. (Default is 1)
"ShowFramerate"			    - Displays the framerate if the value is 1. (Default is 0)
"OldMouseLook"			    - Uses the old mouse look code if the value is 1. (Default is 0)
"NoFunMenus"			    - Only displays the default main menu if the value is 1. (Default is 0)
"RestrictCinematicsTo4x3"	- Adds black bars onto the sides of cinematics on a non 4x3 resolution, if the value is 1. (Default is 0)
"QuickSwitch"			    - Instantly switch between weapons, if the value is 1. (Default is 0)
"UIScale"			        - Scales the in-game HUD. (Default is 0.5)
"UseGotyMenu"			    - Switch between the original main menu and the GOTY version. (Default is based on your version)
"ConsoleBackdrop"           - Swap between 3 different console backdrops: (0) demo, (1) blanktag, and (2) black. (Default is 0)
"BigHeadMode"               - Enable or disable BigHeadMode. (Default is 0)
"DisplayTriggers"           - Shows or hides a physical representation of level triggers. (Default is 0)
"EnableScreenTinting"       - Enable or disable native screen tinting. Disabling will activate an alternate screen tinting. (Default is 1)
"EnableLightScale"          - Enable or disable light scaling. (Default is 1)

Most of these commands are also available in their respective options menu.

-- Windowed Mode
To run in windowed mode either toggle it in-game or, add +windowed 1 to the "Command-Line" textbox in "Advanced" options of the launcher.

-- Known Bugs

Unfortuantely we can't fix everything! Here's a list of known bugs.


Bug: Help I'm stuck!
You can enter in the console (see controls for the console key) `mpclip` to turn on no clip mode. Once you've gotten yourself out of the sticky spot, you can enter `mpclip` in the console to turn off no clip.

Bug: I get a black screen underwater!
This is due to Intel's onboard graphics not liking Direct3D/DirectX7. If your computer has a dedicated gpu, you can try forcing it on by plugging in an external monitor. Or enable "Intel HD Graphics Fix" in Display options.

Bug: The game crashes with "NOLF Error: Couldn't set D3D Emulation mode."
In advanced options of the launcher try checking "Restore Default Options". Also make sure the Display selected is your primary monitor. 

Bug: The game crashes immediately with no error!
Lithtech seems to dislike certain usb devices (like VR headsets or certain logitech devices..) Please try unplugging them before you launch the game.

Bug: Some geometry may cause the player to be pushed or be hard to traverse
There seems to be an issue with the underlying physics engine. We've corrected most of the game breaking issues, but if you find any terrain or doorways that impossible to enter please let us know!

Bug: Game runs really fast on unlocked framerates
The game was designed to work at a locked 60 fps. It is possible to correct most of the speed up issues, but that would be incredibly time consuming, and some of the issues are due to how the engine itself handles physics and sound. 

Bug: Dynamic lighting (flashlights) cause my framerate to dip below 60
On the few systems we tested we encountered an issue with DGVoodoo2. If you're running that software, I'd reccomend you disable it when using this patch.

Bug: The game's window stretches beyond my screen
You'll have to either set display scaling to 100%, or run the game at a lower resolution.

Bug: The game runs slow, and all the text has black boxes around them
If you're running a laptop with a hybrid integrated/dedicated graphics card setup, make sure you force the game to use the dedicated graphics card! Intel integrated graphics seems to have issues running older games. 
If you're running on a desktop, try checking "Restore Default Options" in the advanced section of the launcher. You may to do this twice...

Bug: Weapons sometime disappear during combat!
I've encountered it, but can't for the life of me figure out why it's happening! There's no known fix, but luckily it's only a visual issue that should disappear when you go to another area.

Bug: Big Head Mode has weird hitboxes
Yeaaah..I've tried to make it as close as possible. Hopefully I have another chance to go over it. 
