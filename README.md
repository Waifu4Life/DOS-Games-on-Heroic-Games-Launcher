# DOS-Games-on-Heroic-Games-Launcher

To properly launch DOS games from GOG.com and other places with Heroic Games Launcher


**FAQ:**

Q1- Why do this at all?

A1- Because while WINE is not an emulator, there's still a layer of compatibility needed to run it. DOSBox itself is an emulator and the one that comes with GOG games is the Windows version. Add these two things and you get staudering in these old games sometimes. Using a native Linux DOSBox removes these issues.

Q2- Can you make files for me that are not listed?

A2- No, I only did the ones for the games that I have, but feel free to use one of mine as a template to make your own.

Q3- Some of these games can be played online, can I still do this?

A3- Probably, but you'll need to make your own single.conf file for this.

Q4- Can I submit files for you to add to the list?

A4- Sure, just post a link in the "Issues" of this Github. Mind you, if someone reports that it's not working, then I'll remove it.


**How to:**

Step 1- Install a non-flatpak/non-appimage version of Heroic Games Launcher (https://github.com/Heroic-Games-Launcher/HeroicGamesLauncher/releases)

Step 2- Install a non-flatpak/non-appimage of DOSBox Staging (https://dosbox-staging.github.io/releases/linux/)

Step 3- If you have DOS GOG games, install them using Heroic Games Launcher then hide them (if they're not GOG games, skip to the next step)

Step 4- Rename your DOS game folders 8 characters or less (I was not able to make this work otherwise)

Step 5- Download the zip files from the "Releases" section that you need and unzip the config files into your appropriate game folders (if you want to keep the originals, then back them up first)

Step 6- Using a text editor, edit every "single.conf" file and replace every "full path to your game" for the actual path to your game

Step 7- In Heroic Games Launcher, click on "ADD GAME", type the name of you game, choose "Windows" for the platform and put this in "Select Executable": **/usr/bin/dosbox** , click "Finish"

Step 8- Right click on the new game entry and choose "Settings" and click on the "Advanced" tab

Step 9- In "Game Arguments" enter the following **-conf /full path to your game/game_name.conf -conf /full path to your game/game_name_single.conf -noconsole -c exit**

Step 10- Replace "full path to your game" for the actual path to your game and "game_name.conf" for the name of the Config file of your game and "game_name_single.conf" for the name of the Single Config file of your game
