# osu-keysounds
## About
Gives osu's typing sound effects system-wide on Linux with minimal dependencies. Sound effects can, of course, be replaced.
Note that the sound effects are licensed under [CC-BY-NC 4.0,](https://creativecommons.org/licenses/by-nc/4.0/legalcode) and just [these files](https://github.com/ppy/osu-resources/tree/master/osu.Game.Resources/Samples/Keyboard) converted to `wav`.
## Dependencies
* `basename` for help
* `xset` to get keyrepeat rate, though it shouldn't break if rate is given explicitly
* `awk` for floating-point division to get sleep time from rate
* `grep` for a lot
* `xmodmap` to get keycodes
* `paplay` to play audio
* `xinput` to get key events

## Usage
```
keysounds [OPTIONS]
  -m, --mods, --modifiers     do not ignore modifier keys
  -v, --vol, --volume NUM     sound volume, 1-100, default 60
  -r, --rate NUM              minimum time between sounds in ms, defaults to keyrepeat rate
  -l, --lower, --lowercase    treat everything as lowercase (do not use key-caps.wav)
  -h, --help                  display this help
```
