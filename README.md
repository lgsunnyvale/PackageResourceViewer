# PackageResourceViewer
Plugin to assist viewing and editing package resources in Sublime Text 2 and Sublime Text 3.

## Installation
Note with either method, you may need to restart Sublime Text for the plugin to load properly.

### Package Control
Installation through [package control](http://wbond.net/sublime_packages/package_control) is recommended. It will handle updating your packages as they become available. To install, do the following.

* In the Command Palette, enter `Package Control: Install Package`
* Search for `PackageResourceViewer`

### Manual
Clone or copy this repository into the packages directory. Ensure it is placed in a folder named `PackageResourceViewer`. By default, the Packages directories for Sublime Text 2 are located at:

* OS X: ~/Library/Application Support/Sublime Text 2/Packages/
* Windows: %APPDATA%/Roaming/Sublime Text 2/Packages/
* Linux: ~/.config/sublime-text-2/Packages/

By default, the Packages directories for Sublime Text 3 are located at:

* OS X: ~/Library/Application Support/Sublime Text 3/Packages/
* Windows: %APPDATA%/Roaming/Sublime Text 3/Packages/
* Linux: ~/.config/sublime-text-3/Packages/

## Usage

### Commands
`PackageResourceViewer: Open Resource`:

Command to open the resource. If saved, the correct directory structure will be created in the `Packages` folder. This command will only be displayed if the `single_command` setting is true.

`PackageResourceViewer: View Package Resource`:

Open package resource as read only. This command will only be displayed if the `single_command` setting is false.

`PackageResourceViewer: Edit Package Resource`:

Open package resources as an editable file. Upon execution, this plugin will create a directory (if necessary) as well as save the resource. This command will only be displayed if the `single_command` setting is false.

## Settings
`ignore_patterns`:

A list of regular expressions patterns to ignore. Note that these regular expressions are compared against the file or directory name.

`open_multiple`:

Boolean to keep selection panel open after selecting a resource to open.

`single_command`:

Boolean setting specifying if a single command should be listed in the command palette for viewing and editing files or if multiple commands should be used.
