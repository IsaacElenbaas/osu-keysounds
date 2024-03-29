# osu-keysounds
## About
Gives osu's typing sound effects system-wide on Linux with minimal dependencies. Sound effects can, of course, be replaced.
Note that the sound effects are licensed under [CC-BY-NC 4.0,](https://creativecommons.org/licenses/by-nc/4.0/legalcode) and just [these files](https://github.com/ppy/osu-resources/tree/master/osu.Game.Resources/Samples/Keyboard) converted to `wav`.
## Dependencies
* `basename` for help
* `bash` version 4 or later
* `grep` (optional)
* `paplay` to play audio
* `xinput` to get key events
* `xmodmap` to get keycodes
* `xset` to get keyrepeat rate (optional with `--rate`)

## Usage
```
keysounds [OPTIONS]
  -m, --mods, --modifiers     do not ignore modifier keys
  -v, --vol, --volume NUM     sound volume, 1-100, default 60
  -r, --rate NUM              maximum number of sounds per second, defaults to keyrepeat rate
  -l, --lower, --lowercase    treat everything as lowercase (do not use key-caps.wav)
  -h, --help                  display this help
```
