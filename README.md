# EditorConfig Notepad++ Plugin

This is an [EditorConfig][] plugin for Notepad++.

## Installation

### Install from the Binary Package

Binary package is not ready yet. If you want to install from source, see the
`Install from Source` section.


### Install from Source

Before installation, you must have both [cmake][] and [Microsoft Visual C++][]
installed.

1. Download the [EditorConfig core][] and follow the instructions in the README
   and INSTALL files to compile and install it with Microsoft Visual C++.

2. Download the [EditorConfig plugin for Notepad++][] and extract it.

3. Open your command line prompt, and use `cd` command to switch current
   working directory to the root of the source tree of the Notepad++ plugin.
   Use the following command to generate the project file:

   `C:\path\to\editorconfig-notepad-plus-plus> cmake . -DEDITORCONFIG_CORE_PREFIX="$(The_path_to_EditorConfig_core_prefix)"`

   After this project file is built, double click on the project file and use
   Microsoft Visual C++ to build it.

5. If the build succeeded, you should have `bin\unicode\NppEditorConfig.dll`
   and `bin\ansi\NppEditorConfig.dll` in your build tree. Copy the
   corresponding one (the unicode one if your Notepad++ is unicode version or
   the ansi one if your Notepad++ is ansi version) to your the plugin directory
   of the Notepad++ directory to complete the installation.




[cmake]: http://www.cmake.org
[EditorConfig]: http://editorconfig.org
[EditorConfig core]: https://github.com/editorconfig/editorconfig
[EditorConfig plugin for Notepad++]: https://github.com/editorconfig/editorconfig-notepad-plus-plus
[Microsoft Visual C++]: http://msdn2.microsoft.com/en-us/visualc/default.aspx
