OpenGOAL Flatpak
----------------

Flatpak package for the OpenGOAL launcher.

## Installation

First, [add](https://flatpak.org/setup) the Flathub repository. Then run:

```
$ flatpak install dev.opengoal.OpenGOAL
```

By default, OpenGOAL only has access to the Flatpak application directory. You will need to select your desired game data directory.

To grant access to other directories, you can use [Flatseal](https://flathub.org/apps/details/com.github.tchx84.Flatseal) or the Flatpak override command (e.g., `flatpak override --user --filesystem=<PATH> dev.opengoal.OpenGOAL`)