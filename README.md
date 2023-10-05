# rofi-screenshot-wayland
> Script for taking screenshots on minimalist Linux distributions. Now with support for wlroots based wayland compositors (such as Sway)

Forked from [rofi-screenshot](https://github.com/danrog303/rofi-screenshot).

## Features
1. Using rofi to display screenshot taking menu
2. Allows to take screenshot of whole screen, only selected region (region can be selected using mouse), selected window (using mouse), or the currently active monitor.
3. Saving image as JPG, PNG or copying screenshot to clipboard

## Dependencies
Before you use this application, you need to install the following dependencies - either using your package manager (like apt, pacman) or by manually compiling source codes.

### Wayland
The following dependencies are required for Wayland version:
- rofi (for displaying menus)
- grimshot (for taking the screenshot)
- imagemagick (for converting screenshots to jpg)

### Original
The following are required for the X11 version:
- rofi (for displaying menus)
- slop (for selecting screen regions)
- ffcast (for saving screenshots of entire screen or specified region)
- xclip (for copying image to clipboard)
- libnotify (for sending desktop notifications)
- imagemagick (for converting screenshots to jpg)

## Usage
1. Install required dependecies.
2. Clone this repo
3. Copy the desired script (`rofi-screenshot.sh` or `rofi-screenshot-wayland.sh`) to any directory in your $PATH environmental variable
4. Give the script execution rights by running `chmod a+x rofi-screenshot.sh` or `chmod a+x rofi-screenshot-wayland.sh`
5. Run the script to open screenshot taking tool (or assign the script to a keyboard shortcut to have it always at hand)

## Screenshots
<img alt="Screenshot: rofi-screenshot" src="https://user-images.githubusercontent.com/32397526/148370014-757b1059-3dff-4509-80e0-5db7527eacba.png" width="400">
<img alt="Screenshot: rofi-screenshot" src="https://user-images.githubusercontent.com/32397526/148370019-414ae950-4c3a-4c4a-a4c5-9ba4cdb3960c.png" width="400">
<img alt="Screenshot: rofi-screenshot" src="https://user-images.githubusercontent.com/32397526/148370021-31c5bd97-a76b-4294-9d73-e8144bf65499.png" width="400">

## Technologies used
This script has been written in pure POSIX-compliant Linux shell (`/bin/sh`). Script should run on any Linux distribution where all required dependencies can be installed.