# recktard's fork of st

The [suckless simple terminal](https://st.suckless.org/) with some basic features:

+ Transparency (alpha)
+ Scrollback with mousewheel
+ Clipboard 

## Configuration

Simply modify the `config.h` file. 
Default configuration is stored in `config.def.h`.

## Installation

```
sudo make clean install
```

## Useful keyboard shortcuts

+ Ctrl+Shift+J to zoom out (make text smaller)
+ Ctrl+Shift+K to zoom in (make text bigger)
+ Ctrl+Shift+C to copy
+ Ctrl+Shift+V to paste
+ Select and middle mouse button also copies and pastes

## del key in bash
Add `tput smkx` to your `.bashrc`.\n
The del key does not work out of the box in `st` and therefore this is the easiest workaround.\n
No need of modification if using `zsh`.

## Features not included in st
+ del key not perfectly working in bash (provisional fix)
+ No realignment if st is being resized
+ No select and scroll
+ Endless scrollback (not big of a deal)
+ No vi(m) keybinds
