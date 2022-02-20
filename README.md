This is an extension for Drive Badger. It provides `exclude.list` file, containing a list of exclusions compatible with popular `rsync` program.

The purpose of these exclusions is to decrease the amount of data to be exfiltrated by Drive Badger, and thus to speed up the attack,
by eliminating files and directories, that are not valuable in any way to the attacker:

- hardware drivers, including for common peripheral devices (Creative soundcards, HP printers etc.)
- preinstalled trial versions of Microsoft Office
- preinstalled OEM software (Acer, Dell, Fujitsu etc.) - excluding:
   - antivirus and other security software (see https://github.com/drivebadger/exclude-antivirus repository)
   - OEM games, game launchers and other related tools (see https://github.com/drivebadger/exclude-gaming repository)
   - PDF related software (see https://github.com/drivebadger/exclude-pdf repository)
   - trial versions of image/audio/video recording/editing/streaming software (see https://github.com/drivebadger/exclude-digital repository)

### Installing

Clone this repository as `/opt/drivebadger/config/exclude-oem` directory on your Drive Badger persistent partition.

### More information

- [Drive Badger main repository](https://github.com/drivebadger/drivebadger)
- [Drive Badger wiki](https://github.com/drivebadger/drivebadger/wiki)
- [description, how configuration repositories work](https://github.com/drivebadger/drivebadger/wiki/Configuration-repositories)
