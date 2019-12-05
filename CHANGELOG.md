## [0.2.4] - 2019-12-04
### Added
- optional MQTT messages dump for devices

## Changed
- main script name changed to `tdmgr.py` prior to packaging on PyPI (due to conflicting name with other project)

## [0.2.3] - 2019-11-27
### Added
- ~/TDM directory is created automatically if missing, to prevent logging module crash

### Fixed
- forced RSSI to be cast as int() for some odd cases
- reconnect is now enough to subscribe to new custom patterns (thanks to pgollor)

## [0.2.2] - 2019-11-21
### Added
- Device list now sorts correctly when using diactrics in friendly names
- Some logging features for MQTT and Autodiscovery process
- Toolbar actions now available in device list context menu (#55)
- Preferences dialog: console word-wrap setting and font size and version formatting option for device list
- Clear obsolete LWTs dialog added in MQTT menu
- Save/Clear functions to console

### Fixed
- Power ALL was sending true/false instead of 0/1 (#53)

## [0.2.1] - 2019-11-16
### Fixed
- forced sorting of POWER\<x\> keys when generating toggle actions and drawing state icons
- exception catching when SetOption parsing fails in older Tasmota versions 

## [0.2.0] - 2019-10-02
### Added
- consoles for each device, with colored output to ease reading (needs some polishing), command completion and history
- buttons, switches and relays configuration dialog
- custom widgets in the redesigned device list, including different views

### Changed
- most of the codebase rewritten