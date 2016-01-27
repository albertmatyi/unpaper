# unpaper

A linux bash script for setting wallpapers randomly downloaded from [unsplash.com](http://unsplash.com)

## Usage

`$> unpaper` - downloads a random image and sets it as your background

`$> unpaper -d` - runs the script indefinitely changing the wallpaper every 5
minutes


## Dependencies

* `curl` - for downloading files (alternative might be `wget`)
* `feh` - for setting a wallpaper (can use `nitrogen` as well or others)
* `xorg-xrandr` - for figuring out screen resolution (instead of hardcoding)

## Future

* provide other command line args
* create an *AUR* package out of it (complete the PKGBUILD file & upload)
* add a small UI (`xfltk`, `gtk` or `nwjs.io`)
