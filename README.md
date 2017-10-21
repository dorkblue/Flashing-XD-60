# Flashing-XD-60
Everything I know (limited) about flashing the XD 60 (atmega32u4) with dfu-programmer using the command line.

## Building keyboard firmware (.hex)
[Keyboard Firmware Builder](http://kbfirmware.com/)


## Installing build tools to flash driver?
[Getting Started Build Tools](https://docs.qmk.fm/getting_started_build_tools.html)


## Dfu Programmer Cmd Lines
### Commands
```dfu-programmer --help```
See list of commands for dfu-programmer

### Steps
1. `dfu-programmer atmega32u4 erase --force --debug 1000`

Erase existing memory 

2. `dfu-programmer atmega32u4 flash keymap.hex --debug 1000`
Flash with .hex keymap

3. `dfu-programmer atmega32u4 reset --debug 1000`
Reset

