# unpaper

A linux bash script for setting wallpapers randomly downloaded from [unsplash.com](http://unsplash.com)

## Usage

`$> unpaper` - downloads a random image and sets it as your background

`$> unpaper -d` - runs the script indefinitely changing the wallpaper every 5
minutes


## DEPENDENCIES

* `curl` - for downloading files (alternative might be `wget`)
* `feh` - for setting a wallpaper (can use `nitrogen` as well or others)
* `xorg-xrandr` - for figuring out screen resolution (instead of hardcoding)
