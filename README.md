# Flashing-XD-60
Everything I know (limited) about flashing the XD 60 (atmega32u4) with dfu-programmer using the command line.

## Building keyboard firmware (.hex)
[Keyboard Firmware Builder](http://kbfirmware.com/)


## Installing build tools to flash driver?
[Getting Started Build Tools](https://docs.qmk.fm/getting_started_build_tools.html)


## DFU-Programmer Cmd Lines
### Commands
```dfu-programmer --help```
See list of commands for dfu-programmer

### Steps
1. Erase existing memory

> ```dfu-programmer atmega32u4 erase --force --debug 1000```

2. Flash with .hex keymap

> ```dfu-programmer atmega32u4 flash keymap.hex --debug 1000```

3. Reset

> ```dfu-programmer atmega32u4 reset --debug 1000```

## Links that helped
[https://github.com/qmk/qmk_firmware/issues/122](https://github.com/qmk/qmk_firmware/issues/122)

[https://imgur.com/a/IcT03#vxvPgdU](https://imgur.com/a/IcT03#vxvPgdU)
