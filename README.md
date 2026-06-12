# Zed Conifg

This is my zed editor config, which works across Windows, Max and Linux.

## Clone this repo

For Windows

```powershell
git clone ~/AppData/Roaming
mv my_zed_config Zed
```

For Mac and Linux

```bash
git clone ~/.config/zed/
mv my_zed_config zed
```

## Zed Config File Path

Windows

```text
~/AppData/Roaming/Zed/settings.json
~/AppData/Roaming/Zed\keymap.json
```

MacOS & Linux

```text
~/.config/zed/settings.json
~/.config/zed/keymap.json
```

## Print All Extensions

Powershell

```powershell
Get-ChildItem "$env:LOCALAPPDATA\Zed\extensions\installed" -Name
```

Bash

```bash
# Ubuntu
ls ~/.local/share/zed/extensions/installed/ | awk '{print "  \"" $1 "\": true,"}'

# macOS
ls ~/Library/Application\ Support/Zed/extensions/installed/ | awk '{print "  \"" $1 "\": true,"}'
```
