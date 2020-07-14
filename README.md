# Minimal OS

## Before beginning... ##
This is just almost a pure vanilla AOSP fork but, I got some stuff that I found useful. Not a whole has been changed either.

## Building Android ##
[Setting Up Build Environment](https://raw.githubusercontent.com/nathanchance/Android-Tools/master/Guides/Building_AOSP.txt) | [Setting up WSL on Windows 10](https://sourajitk.github.io/posts/wsl-2-how-to/)

## Repo Init ##
```bash
repo init -u https://github.com/Minimal-OS/manifest.git -b 10
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```

## Building for your device ##

If you are building for a Pixel device, you can comment out the repos for your device's codename in ```remove.xml``` and then typing in the above repo sync command.

If you are building for the Essential PH-1, I am tracking a pure AOSP tree I modified slightly released by [Essential Products OSS team](https://github.com/EssentialOpenSource). 

Feel free to modify it and anything in here, in anyway you desire :D