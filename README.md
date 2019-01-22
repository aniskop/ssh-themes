# SSH Themes

This project is a set of color themes for SSH terminal window. Colors of all themes are borrowed from popular IDE color themes as-is or with slight modifications. All colors are picked so that traditional Linux terminal colors are still recognizable.

Each theme comes as a Windows registry (.reg) file, which is suitable for WinSSHTerm and PuTTY SSH clients. All themes have references to their origin.

Supported themes:
* [PuTTY default terminal colors](./putty)
* [Cobalt2](./cobalt2)
* [Darcula](./darcula)

# Installing and using color theme in WinSSHTerm

To install a color theme:
1. Open menu File > Preferences.
2. In the "Color Theme" block click "Edit".
3. Select one of the custom themes (default names are Custom1, Custom2 etc).
4. Click "Load .reg file" and select the .reg file of the color theme to import.
5. (Recommended) Click "Rename" to change theme name in WinSSHTerm.

To use a color theme:
1. Open menu File > Preferences.
2. Select the color theme from the "Color Theme" dropdown.
3. Click "OK".

From now the theme will be in use for all new sessions. Sessions opened before changing the color theme will stay intact.

# Installing and using color theme in PuTTY

1. In the theme .reg file change "WinSSHTerm" to a name of the saved PuTTY session.
2. Import the .reg file.

For instance, let's assume PuTTY session name is "My_Session" and .reg file contains:
```
[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\WinSSHTerm]
```

With a text editor in the .reg file change "WinSSHTerm" to "My_Session", save changes and double-click the .reg file to import it to the Windows registry. From now the color theme will be used for the specified PuTTY session.
