MIDI-to-Keypress
================

Takes MIDI events and turns them into keypresses.
Renewed from: https://github.com/xobs/midi-to-keypress/releases for new version of Rust version and Rust libraries.

Also, this version uses `#` character for delimiting config file, instead of ` ` character, because `space` key is very commonly used in daily typing or controlling.

Building
--------


`cargo run` or `cargo build` for debug build

`cargo build --release` for release build


Usage
-----

- "cargo run -- --list" : list all midi devices
- "cargo run -- --device [device-name]" : Specify a device to use as an input
- "cargo run -- -f mappings/sharps.txt" : Specify a mapping file to use

Mapping Files
-------------

Mapping files are located in `mappings` folder.

- `sharps.txt` : `sdf jkl` are respectively mapped from F4 to B4, with sharp notes
- `sdf-jkl.txt` : `sdf jkl` are respectively mapped from, C4 to B4, all white notes