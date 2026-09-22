# FocusME
Helper script to focus open Linux/X window apps or launch another instance if window is already active or not found. 
You can forget the hordes of orphaned terminals or myriads of app windows.

It works by querying the open window names/classes for a string, then:

- If found it activates/focuses it.
- If not found it will launch the specified command.
- If the window is found and it's active it will me minimized.

## Required packages
- Requires [xdotool](https://github.com/jordansissel/xdotool) to work

## Usage, examples
```
focusme <windowname> <command_to_launch>

windowname - text part of the window name
command_to_launch - the command to launch if window not found or already active

focusme terminal xfce4-terminal
focusme firefox "firefox -P MAIN"
```

## Fork info
This version if forked from the [original repo](https://github.com/dixflatlinr/FocusME) as I didn't like the original behaviour of opening new instance of the window if one is currently focused. This version minimizes the window.