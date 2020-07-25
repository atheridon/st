# Atheridon's fork of st

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

## del key not working
Add `set enable-keypad on` to `/etc/inputrc` or `~/.inputrc`.

## Features not included in st
+ No realignment if st is being resized
+ No select on scroll
+ Endless scrollback (not big of a deal)
+ No vi(m) keybinds
