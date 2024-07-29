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

## Known Issues

Since this is a Tauri v1 application, it relies on webkit2gtk, which has a known issue with NVIDIA graphics.
This issue can be fixed by disabling the WebKit's DMA buffer renderer, either using [Flatseal](https://flathub.org/apps/details/com.github.tchx84.Flatseal), or the command line:

```
$ flatpak override --env=WEBKIT_DISABLE_DMABUF_RENDERER=1 dev.opengoal.OpenGOAL
```