# Improved-Player-Cmus
My version of the player-cmus script based on the [player-cmus script](https://github.com/polybar/polybar-scripts/tree/master/polybar-scripts/player-cmus) in the polybar script repository.

## Installation
Simply download the script to your polybar-scripts directory and place the module within your polybar config file. Make sure to add the module to your bar by typing the name of the module in the modules-center shown below.
```ini
[bar/example]
modules-left = ...
modules-center = player-cmus
modules-right = ...
```

## Changes
- Changed the numbers for the status of the song to different titles such as Now Playing, Paused, Stopped.
- Swapped the modules for skipping songs and replaying previous songs

```ini
[module/player-cmus]
type = custom/script
exec = ~/polybar-scripts/improved-player-cmus.sh
interval = 5
click-left = cmus-remote -r &
click-right = cmus-remote -n &
click-middle = cmus-remote -u &
```
