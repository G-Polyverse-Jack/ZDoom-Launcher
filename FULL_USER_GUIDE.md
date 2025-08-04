## ZDoom Launcher 1.0 - by G Polyverse Jack
	FULL GUIDE

	**CHAPTERS**
1. Using menus - Multiple choice menus; input section menus
2. Profiles - Default profile; current profile; username
3. Profile manager
4. Main menu - Single player launch; multiplayer menu; seeing current version; other options
5. Adding files submenu
6. Multiplayer menu
	I. - join submenu
	II. - host submenu
7. Appendix - Compatibility; custom commands



	**1. USING MENUS**

a) MULTIPLE CHOICE MENUS
You will mainly see multiple choice menus with options highlighted with a number or letter between square brackets before it.
Example:

         ZDOOM LAUNCHER

        You're using Guest profile
        [1] Single player
        [2] Multiplayer (net-game)
        [3] Change profile
        [4] Help
        [5] Quit Doom Remake 4 Launcher

Type and enter the number to select an item from the menu _

To select an option you just need to type the value between the square brackets related to the wanted option and then press enter. The option values are not case sensitive.
You will see your input before "entering" it right after the menu message or in the lowest line.

Comfirmation dialog messages work the same way.
Example: 

        Restore default profile:
Are you sure? Some progress might be deleted [Y/N] _

It means that you can confirm by entering "Y" and denying by entering "N"

b) INPUT SECTION MENUS
You will also come across menus in which you have to enter an input that is requested.
Example: 

Type the name of the profile file form the list without extension _

This means that you need to type the value you are requested and then enter it. This time the input is case sensitive and you shoud type exactly, taking care of spaces and symbols, your desired input.
If you would like to go back, you will usually see the current value selected or a list of values, which you can copy and paste it by selecting it with the mouse. Sometimes entering blank values can trigger some errors that will reset the input to the last selected.


	**2. PROFILES**

A profile is a system of selecting a game configuration file (*.ini) associated with an user name, so that you can be aware of what you will load. Profiles can be changed and made with the profile manager tool.

a) DEFAULT PROFILE
It comes with a pack dedicated to (G)ZDoom itself or a particular game/mod that has its data separated
There is a default configuration file name and it is associated with the "Guest" user name
It is designed to be used as a temporary profile and progress can be saved to it. You can restore this progress to the very default with the profile manager tool.

b) CURRENT PROFILE
When loading the launcher with the Guest/default profile already selected you will see a confirmation dialog message asking you whether to change or keep using the default profile. You can see your current profile in the main menu, which displays the associated username.

c) USERNAME
The username is a sort of identifier for the profile. If you're using ZDoom Launcher to run different games/mods it is recommended to specify which game the profile is designed for. If you're using ZDoom Launcher to run a separated game/mod you should just specify who the user is.
Usernames can be any input wanted, unlike configuration file names that cannot include spaces.


	**3. PROFILE MANAGER**

It is a tool that helps you manage profiles.
Here's the main menu interface of the profile manager:

        PROFILE MANAGER

        Current profile:
        Guest

        File: zdoom.ini

        [1] Change profile
        [2] Create own profile
        [3] Change to guest
        [4] Edit current profile file and user name
        [5] Restore guest profile progress
        [6] Import/export external profile
        [7] Save and go back to main menu
        [8] Delete current profile

_

It displays both the username and configuration file id of the current profile selected.

1) CHANGE PROFILE
Shows a list of configuration files available in the (G)ZDoom-folder\Profiles\ folder.
Asks you to enter the filename without (.ini) extension to change to the related profile.
To cancel the operation you can enter a blank or non-existing input after which yoi will be showed an error and the profile will not be changed.

2) CREATE OWN PROFILE
This feature makes you create a copy form the default profile (whith or without progress) to a custom one with custom file name and username. It is designed mostly to make a player profile for separated games/mods.
You are not allowed to use spaces for the file name as it would trigger an error screen and cancel the operation.
If you want to duplicate the current profile to a custom one you need to use the "Import/export profile" feature.

3) CHANGE TO GUEST
Changes to Guest (default) profile automatically.

4) EDIT CURRENT PROFILE FILE AND USER NAME
Lets you change the filename and username. Make sure to type legal filenames.

5) RESTORE GUEST PROFILE PROGRESS
It overwrites the default profile's configuration file that potentially had progress saved with a clean defult one

6) IMPORT/EXPORT EXTERNAL PROFILE
This feature lets you create a new profile from a configuration file located on any path or to export your current profile file to a custom path to bring it wherever you want or to shere it with other people. Make sure to type the path between quotes to avoid issues related with folders or files that contain spaces. If you import a file you can give it a custom filename and create a new username. If you Export it, you will export the current one to a path. You can change the filename by typing it after the folder path by adding the *ini extension. However no username will be saved after the exportation and if you enter a non-existing path, no files will be saved.
If you want to duplicate the current profile to a custom one you need to export the current profile and then import it again.

7) SAVE AND GO BACK TO MAIN MENU
Goes back to the main menu.

8) DELETE CURRENT PROFILE
Deletes the currently selected profile (both configuratin file and username) and changes to guest. You cannot delet the Guest/default profile.


	**4. MAIN MENU**

It's the first menu that shows when you start the launcher and is lets you select the playing mode or open the profile manager.

1) SINGLE PLAYER LAUNCH
Lets you start the game/mod offline to play alone and it loads the configuration file of the currently selected profile.

2) MULTIPLAYER MENU
Opens a menu dedicated to multiplayer online games (see (G)ZDoom availability for online games).

3) SEEING CURRENT VERSION
Wonder what is the current ZDoom Launcher version you're using? Just type and enter "V".

4) OTHER OPTIONS
You can open the profile manager tool if you selectthe "Change profile" option.
"Help" option displays you some basic instructions on how to use ZDoom Launcher and you can quit it by entering "5".


	**5 ADDING FILES SUBMENU**

It's the sub menu that opens when you select the single player experience or join a multiplayer game.
It is designed for loading additional files (usually WADs) along with the game/mod. It remembers the currently set files and you can choose whether to load the game with the files or ignore them and keep them for a following time, change the selected files or clear the list. If the files are located in the (G)ZDoom folder you can just type their names (with extension). If the files are located anywhere, you can paste the full path. Make sure to use quatation marks to avoid issues with filenames with spaces.


	**6. MULTIPLAYER MENU**

Here you can choose whether to join or host a multiplayer online game.

	I. JOIN SUBMENU
It lets you set the the IPv4 address and the port of the host.
After choosing to connect to the game you will be shown the adding files submenu to load potentially necessary files that the host requires you to load.

	II. HOST SUBMENU
This submenu lets you select intuitively the parameters of the game you want to host. It is inspired by the Death Manager, A.K.A. DM.EXE in MS-DOS.
Here's the interface:

        HOST GAME
        Inspired by Death Manager! (DM.exe)

        [0] Back
        [p] Port: 5029
        [n] 2 players  [g] Game type: Deathmatch
        [s] Saved game:
        [1] Load saved game? no
        [2] Warp to E1M1  [3] Skill 3
        Miscellaneous
        [4] No monsters? yes
        [5] Timer off  [t] 20  minutes
        [6] Respawning? no
        [a] Add files
        [7] Load files? no
        [c] Additional custom command:

                 [10] GO!

_

p) PORT
Lets you input the host port (default is 5029).

n) PLAYERS
Lets you input the number of players of the game you want to host.

g) GAME TYPE
Lets you select the game type (more info on doom wiki fandom).

s) SAVED GAME
Lets you input the *zds file of saved progress from a previous saved game.

1) LOAD SAVED GAME?
Switches whether to load the saved game and disable warping and skill selection or not.

2) WARP TO
Opens a submenu that helps you select a map to start the game at. You can choose a map configuration or input the full name of the map.

3) SKILL
Lets you input the skill (difficulty) number.

4) NO MONSTERS?
Switches whether to clear the maps from monsters or not.

5) TIMER
Switches whether to turn on or off the timer that changes automatically to the following map after the chosen amount of time.

t) MINUTES
Lets you input the amount of minutes for the timer.

6) RESPAWNING?
Switches whether to let mosnters respawn or not after being killed

a) ADD FILES
Lets you input the additional files to load, after displaying the currently selected files.

7) LOAD FILES?
Switches whether to loat the selected files or not.

c) ADDITIONAL CUSTOM COMMAND
Lets you input additional command line parameters. They will be shown and remembered after the input.

10) GO!
Launches the game with the chosen parameters (and the current profile's configuration file).


	**7. APPENDIX**

a) COMPATIBILITY
ZDoom Launcher is the same for ZDoom and GZDoom except thet for GZDoom there will be an additional file that gives the instruction to run the correct executable file. Both ZDoom and GZDoom can be in the same foldder and ZDoom Launcher can be loaded normally.

b) CUSTOM COMMANDS
If you're a developer and want to use additional command line parameters for a single player game you can set them in the command.bat batch file located in the "launcher" folder.


