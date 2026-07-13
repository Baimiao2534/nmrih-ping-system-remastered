# NMRiH Ping System (Remastered)

> [!WARNING]
> This is a remastered fork of [dysphie/nmrih-ping-system](https://github.com/dysphie/nmrih-ping-system).
> The original plugin is **unmaintained since Torn Banner's acquisition of the game**, as declared by the original author on GitHub.
> This remaster was created to keep the plugin usable on current NMRiH dedicated servers.

## Overview

This plugin allows players to point at the world and create a visual and audible ping that can be seen and heard by other players. The ping can be used to communicate locations, objectives, enemies, items, or anything else in the game world.

This remastered version is maintained by **Baimiao2534** and continues to receive updates and Chinese localization improvements.

## Credits

- **Original Author**: [dysphie](https://github.com/dysphie)
- **Original Repository**: [dysphie/nmrih-ping-system](https://github.com/dysphie/nmrih-ping-system)
- **Remastered by**: [Baimiao2534](https://github.com/Baimiao2534)

## Requirements

- [SourceMod 1.12](https://www.sourcemod.net/downloads.php?branch=stable) (1.11 will work but with degraded performance)
- (Optional) Client Preferences extension and plugin to allow players to hide pings (bundled and enabled with SourceMod by default)

## Installation

- Grab the latest ZIP from releases
- Extract the contents into `addons/sourcemod`
- Reload your translations: `sm_reload_translations` in server console
- Load the plugin: `sm plugins load nmrih-ping`

## Directory Structure

```
addons/sourcemod/
├── plugins/
│   └── nmrih-ping.smx
├── scripting/
│   └── nmrih-ping.sp
└── translations/
    ├── ping.phrases.txt       (English)
    ├── chi/
    │   └── ping.phrases.txt   (Simplified Chinese)
    └── zho/
        └── ping.phrases.txt   (Traditional Chinese)
```

## Usage

A. Open the voice menu (Default: `3`) and press the Use key (Default: `E`)

B. Bind a key to the `sm_ping` command. For example:

```
bind mouse3 sm_ping
```

## Client Preferences

Players can toggle seeing pings via `sm_settings` -> `Player Pings`

## Translations

This remastered version includes translations for:

- English
- Simplified Chinese (chi)
- Traditional Chinese (zho)

## License

This plugin is licensed under the **GNU General Public License v3.0 (GPLv3)**, inherited from the original work by dysphie.

- You can use, modify, and distribute this plugin as long as you follow the terms and conditions of the license.
- A copy of the license can be found in the [LICENSE](LICENSE) file.
- Source code modifications must be released under the same GPLv3 license.

For the full license text, see <https://www.gnu.org/licenses/gpl-3.0.html>.
