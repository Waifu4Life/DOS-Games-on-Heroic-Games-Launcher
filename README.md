# DOS-Games-on-Heroic-Games-Launcher

To properly launch DOS games from GOG.com and other places with Heroic Games Launcher

Step 1- Install a non-flatpak/non-appimage version of Heroic Games Launcher (https://github.com/Heroic-Games-Launcher/HeroicGamesLauncher/releases)

Step 2- Install a non-flatpak/non-appimage of DOSBox Staging (https://dosbox-staging.github.io/releases/linux/)

Step 3- If you have DOS GOG games, install them using Heroic Games Launcher then hide them (if they're not GOG games, skip to the next step)

Step 4- Rename your DOS game folders 8 characters or less (I was not able to make this work otherwise)

Step 5- Download the zip files from the "Releases" section that you need and unzip the config files into your appropriate game folders

Step 6- Using a text editor, edit every "single.conf" file and replace every "full path to your game" for the actual path to your game

Step 7- In Heroic Games Launcher, click on "ADD GAME", type the name of you game, choose "Windows" for the platform and put this in "Select Executable": **/usr/bin/dosbox** , click "Finish"

Step 8- 
