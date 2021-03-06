![banner](http://aimtux.net/images/banner.png)

===================

[![Join the chat at https://www.gitter.im/AimTuxOfficial/lobby](https://img.shields.io/gitter/room/TechnologyAdvice/Stardust.svg?style=flat-square)](https://www.gitter.im/AimTuxOfficial/lobby)

Want to chat or play with other AimTux users? Join us on Gitter!

## What is AimTux?

AimTux is a fully featured internal hack for *CounterStrike : Global Offensive* written in C++.


## Compiling

**Note:** _Do NOT download or compile as the root user_

#### Download the dependencies required to build AimTux:
__Ubuntu-Based / Debian:__
```bash
sudo apt-get install cmake g++ gdb git libsdl2-dev zlib1g-dev libxdo-dev
```
__Arch:__
```bash
sudo pacman -S base-devel cmake gdb git sdl2 xdotool
```
__Fedora:__
```bash
sudo dnf install cmake gcc-c++ gdb git libstdc++-static mesa-libGL-devel SDL2-devel zlib-devel libxdo-devel libX11-devel
```

__Gentoo:__
```bash
sudo emerge cmake dev-vcs/git gdb libsdl2 mesa xdotool
```

To build AimTux, you require at least (`GCC / G++ v6`) otherwise it will error, to check your gcc / g++ version, run the command 
`
gcc -v
`
and it will tell you on the bottom line the version, if it is not at least v6.0, you will need to follow [this](https://github.com/AimTuxOfficial/AimTux/wiki/Updating-your-compiler) wiki page on how to update.

===================

#### Download AimTux:

```bash
git clone --recursive https://github.com/kwibjo/AimTux
```

```bash
cd AimTux
```

===================

#### Generate a makefile

```bash
cmake .
```

#### Compile with make

**Note:** _The `4` in the command below specifies the amount of cpu "threads" or "cores" you wish to compile with (more = faster)._

```bash
make -j 4
```

## Injecting

First of all, make sure CSGO is open, it doesn't matter whether you're in game or not.

Navigate to the directory where AimTux was built if you haven't ready.

```bash
cd AimTux
```

Now, you can inject the hack with the `load` script

```bash
./load
```

You might be prompted to enter in your password, this is because the injection script requires root access.

You should see a lot of text being printed out, most of which is not important,

If the injection was successfull you'll see a message at the bottom saying `Successfully injected!`, however, if the message says `Injection failed`, then you've most likely done something wrong.

Now, go back into csgo, if you're in the main menu of the game you should see the AimTux banner in the top left like so:

![this](http://aimtux.net/images/screenshot4.png)

## Using the hack

Now that AimTux has been injected into the game, press <kbd>Insert</kbd> on your keyboard to open the hack menu (<kbd>FN</kbd>+<kbd>Delete</kbd> if you're using a laptop).

If you want to change skins, create and load configs or open the player list, you can find those buttons at the top of the screen.

## Unloading the hack

If you wish to unload the hack from the game, you can do so by entering the command:

```bash
./uload
```

## Updating AimTux

We add and improve and fix things almost every day with AimTux. We don't have a fixed release schedule, we just add things to it when they're ready. Because of this, AimTux will need to update a lot.

If you don't update once a day then we recommend at LEAST update once a week, and ALWAYS update after a CSGO update, just to make sure we fix anything that's broken.

We provide a script included in the AimTux folder that updates AimTux for you. To use it, just run:

```
./update
```

And it will download and compile without any effort. Once it's done, happy hacking!

## Video Tutorial for dummies

[![tutorial](http://img.youtube.com/vi/bkEj57BviM8/0.jpg)](https://www.youtube.com/watch?v=bkEj57BviM8)

## Configs

Configs are stored in a hidden directory in your home folder. Specifically 

```
~/.config/AimTux
```

Each `config.json` is stored in a seperately named folder (The name you see in-game, in the config window). 

To add a config, create a folder inside of the `~/.config/AimTux` folder with a name of your choice, and paste the `config.json` inside of that folder.

To see hidden folders inside your home folder, press <kbd>CTRL</kbd>+<kbd>H</kbd> when using a file manager.

## Contributing to AimTux

If you wish to contribute code to this opensource project, please keep some things mind before creating a *pull request*:
 - Make sure you're using the correct [code style](https://github.com/AimTuxOfficial/AimTux/wiki/Code-Style).
 - Make sure your commits are clean and straight forward ( no junk commits )
 - Explain what you've done in your pull request.


## Screenshots

![menu](http://aimtux.net/images/screenshot1.png)
![skins](http://aimtux.net/images/screenshot2.png)
![esp_chams](http://aimtux.net/images/screenshot3.jpeg)

## Credits
Special thanks to [@aixxe](http://www.github.com/aixxe/) ([aixxe.net](http://www.aixxe.net)) for the skin changer and with the initial project, as well as helping this project with source code (Available on [@aixxe's](http://www.github.com/aixxe/) github page.)

This project was also originally based upon Atex's [Linux Basehook](http://unknowncheats.me/forum/counterstrike-global-offensive/181878-linux-basehook.html).
