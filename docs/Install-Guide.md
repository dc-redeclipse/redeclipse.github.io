---
title: Install Guide
layout: docs
origfile: Install-Guide.md
origtitle: Install-Guide
permalink: /docs/Install-Guide
redirect_from:
  - /docs/Install_Guide/
  - /wiki/Install_Guide/
---
* TOC
{:toc}
## Windows
- [Download the installer](/download/windows) and run it.
- Follow the installation prompts.
- You can now access Red Eclipse from your start menu.

If you get a permission denied error during install, right click the installer and [Run as Administrator](http://windows.microsoft.com/en-us/windows7/how-do-i-run-an-application-once-with-a-full-administrator-access-token). Alternatively, you can change the install location to a user-writable folder (like "[My] Documents") during the install process.

## GNU/Linux or BSD
### AppImage
- [Download the stable AppImage](/download/appimage)
- After download, give the AppImage executable permissions through your file manager or using the terminal command `chmod +x redeclipse-*.AppImage`
- You can then run Red Eclipse by double-clicking the AppImage or executing it from a terminal.

[More information and options](AppImages).

### Standard Package
- Install Red Eclipse's dependencies.
    - Debian/Ubuntu: `sudo apt-get install curl libsdl2-mixer-2.0-0 libsdl2-image-2.0-0 libsdl2-2.0-0`
    - Fedora: `dnf install curl SDL2 SDL2_mixer SDL2_image`
- [Download the tarball](/download/linux), move it to your home directory, and extract it with your file manager, an archive utility, or the terminal command `tar -jxvf redeclipse_X.Y.Z_nix.tar.bz2`.
- Enter the extracted folder (redeclipse-X.Y.Z) and run `redeclipse.sh` to launch Red Eclipse.

### From Source
- Install additional dependencies to compile with:
    - Debian/Ubuntu: `sudo apt-get install libsdl2-mixer-dev libsdl2-image-dev libsdl2-dev libfreetype-dev libopenal-dev libsndfile-dev`

From the command line:
- Clone the repository and its submodules with `git clone --recurse-submodules https://github.com/redeclipse/base`
- Enter the working directory with `cd base`
- Compile with `make -C src install -jN`, with `-jN` being set to the number of cores your CPU has (e.g. `-j4` for a quad core system)
- Enter the source directory with `cd src`
- Run the game with `./redeclipse.sh`

## If you get stuck
Don't panic! If you have trouble working out how to install and run the game, you can get assistance on our [Discord](/discord) or [Discussions](/discuss). Please be ready to provide as much information as possible, especially what operating system you're on and specifically which package you're trying to install!

## Important Notice About Unofficial Packages
Red Eclipse is available only through the official installation methods described on this page or via **[Steam](/steam)**.
Packages found on Flathub, Snap, Flatpak, AUR, Linux distribution repositories, the Ubuntu Software Store, or any other third-party source are not official, not maintained, and not supported by the Red Eclipse development team.h
These unofficial packages may be outdated, incomplete, or insecure, and can cause issues that we cannot assist with.
For the best experience and to ensure you're receiving verified, up-to-date builds, please install Red Eclipse exclusively through the official methods provided here or via **[Steam](/steam)**.
