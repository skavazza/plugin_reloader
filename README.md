# Plugin Reloader

**Plugin Reloader** is a QGIS plugin designed specifically for Python Plugin Developers. It allows you to reload a chosen plugin with a single click or keyboard shortcut, significantly speeding up the plugin development process.

## Features

- **One-Click Reload**: Instantly reload your active plugin during development without restarting QGIS.
- **Keyboard Shortcut**: Use `Ctrl+F5` to quickly reload the most recently configured plugin.
- **Recent Plugins List**: Keeps track of recently reloaded plugins for easy switching, and allows configuring the history length.
- **Extra Pre-reload Commands**: Execute custom CLI commands (such as `make dclean`, `pb_tool deploy`, or custom shell scripts) right before the plugin is reloaded.
- **Customizable Toolbar**: Choose whether to display text beside the toolbar icon or just the icon itself.
- **Compatibility**: Fully supports QGIS 3.x and Qt6.

## Installation

The easiest way to install Plugin Reloader is through the official QGIS Plugin Repository:

1. Open QGIS.
2. Go to **Plugins -> Manage and Install Plugins...**
3. Search for "Plugin Reloader".
4. Click **Install Plugin**.

Alternatively, you can clone the source code into your QGIS plugins folder.

## Usage

1. Click on the **Plugin Reloader** menu from the QGIS toolbar (or from the `Plugins` menu).
2. Choose **Reload a plugin...** or select one from your previously reloaded plugins list.
3. Once a plugin is set up, you can simply click the main **Plugin Reloader** icon in the toolbar or press `Ctrl+F5` to reload it instantly.

## Configuration

You can access the configuration dialog by clicking **Configure...** in the Plugin Reloader menu. Here you will find several options:

*   **Notifications**: Enable or disable pop-up confirmation messages when a plugin reloads successfully.
*   **Recent Plugins Count**: Adjust the number of recent plugins shown in the dropdown menu.
*   **Toolbar Appearance**: Toggle whether text is displayed alongside the main toolbar button.
*   **Extra Commands**: Define shell commands to run automatically before the reload process. Two placeholder variables are available for convenience:
    *   `%PluginName%` - Resolves to the name of the selected plugin.
    *   `%PluginPath%` - Resolves to the absolute path of the selected plugin's standard installation directory.

## Links & Contact

- **Original Author**: Borys Jurgiel
- **Email**: qgis@borysjurgiel.pl
- **Homepage & Source Code**: [https://github.com/borysiasty/plugin_reloader](https://github.com/borysiasty/plugin_reloader)
- **Issue Tracker**: [https://github.com/borysiasty/plugin_reloader/issues](https://github.com/borysiasty/plugin_reloader/issues)

## License

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version. See the [LICENSE](LICENSE) file for more details.
