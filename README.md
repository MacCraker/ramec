<p align="center">
    <img src="https://github.com/MacCraker/ramec/raw/main/ramec.png">
</p>

---

ramec is a fork of Crustacean by o7moon, and is a program that allows installing mods for crab game into crab game. It has its own gui, while also allowing support for using a url to install somebodies own mod. 

# Usage
## Installation
 ~~- To install, download a build from [Releases](https://github.com/o7Moon/Crustacean/releases). For Windows users, download the .exe file, for linux users download the extensionless file.~~
 ~~- Next, run the executable. For windows users there may be a "Windows protected your PC" popup message. However, this is caused by an unsigned executable, and signing one can cost some money, so for now just to click "More Info" and then "Run anyway". You will only have to do this once.~~
 ~~- Afterwards, if your game is installed via steam, ramec should find the installation directory of crab game. However, double check it and change the directory if it is incorrect. You can then check the checkboxes of the mods you want, and when you press install, it will install BepInEx 577 and the selected mods (if any).~~
 ~~- As there is a custom uri handler, it needs to know the executable location for it to work. If you move the executable, you will need to run it again (you don't need to press install).~~ builds coming soon

## Using a url to install a mod
 - ramec has support for installing a mod using a url. To install a mod/create a url that can install a mod, the format looks like this: `crustacean://installMod/link/to/your/mod.dll`. 
 Notes: First, this will only support dll files, so no zips. Also, I have not changed the name of this for compatibility reasons.

# FAQ:
### The linux version installs, but the mod doesn't work.
To do this, you will need to enable proton for crab game, and and a dll override for `winhttp.dll`. You can find instructions for adding the dll override here: (https://docs.bepinex.dev/articles/advanced/proton_wine.html). It may be likely that, in the future, the mod can do this automatically.

### Why "ramec"?
Take "Crab Game", but make it start with an R (as in rust), so "rab game". Then, might as well remove the first letter of the other word, so "rab ame". Remove the 3rd letter of each so its shorter and combine them to get "rame". Then, add c at the end, because one of my usernames is koteyka, but ramek looks weird so a C is used to substitute the K, and you get "ramec". I only took *slight* insperation from o7 for making the name a combination of a few things.

### Why does the program use o7moon's `system uri` instead of the official crate?
The official crate is 5 years old and fails to compile. There is a fork with updated dependencies which does successfully compile to linux, but it still wouldn't compile to windows, so o7moon made their own.
