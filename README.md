OpenGOAL Flatpak
----------------

Flatpak package for the OpenGOAL launcher.

## Installation

1. [Add the Flathub repository](https://flatpak.org/setup) if you haven't already.
2. Install the OpenGOAL Flatpak package:

```
$ flatpak install dev.opengoal.OpenGOAL
```

## Usage Notes

By default, OpenGOAL only has access to the Flatpak application directory. You will need to select your desired game installation directory.

**Important:**

Game compilation currently only works if the selected game data directory is the base Flatpak directory:
```
/home/$USER/.var/app/dev.opengoal.OpenGOAL
```