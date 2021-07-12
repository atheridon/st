# Fork of st

The [suckless simple terminal](https://st.suckless.org/). 

## Patches applied

+ alpha
+ blinking cursor
+ clipboard 
+ externalpipe
+ scrollback 
+ newterm

## Configuration

Simply modify the `config.h` file. 
Default configuration is stored in `config.def.h`.

## Installation

```
sudo make clean install
```

## Useful keyboard shortcuts

+ Alt+o to open URLs (need script [st-urlhandler](https://github.com/flolesko/scripts/blob/master/st-urlhandler)! -> change openurlcmd in config.h)
+ Alt+l to copy URLs (need script [st-urlhandler](https://github.com/flolesko/scripts/blob/master/st-urlhandler)! -> change copyurlcmd in config.h)
+ Ctrl+Shift+J to zoom out (make text smaller)
+ Ctrl+Shift+K to zoom in (make text bigger)
+ Ctrl+Shift+C to copy
+ Ctrl+Shift+V to paste
+ Select and middle mouse button also copies and pastes

## del key not working
Add `set enable-keypad on` to `/etc/inputrc` or `~/.inputrc`.

## st in combination with the suckless scroll program

You can also find the suckless scroll program in this repository which,
when enabled in the st config.h file, will add scrollback to st and text 
will NOT be cut off anymore when resizing the terminal window. BUT scroll 
is still experimental and therefore contains bugs.

### How to install scroll

```
cd scroll
sudo make clean install
```
