# AutoHotkey

[AutoHotkey](https://www.autohotkey.com/) is a free, open-source scripting language for Windows that allows users to easily create small to complex scripts for all kinds of tasks such as: form fillers, auto-clicking, macros, etc.


## Create Scheduled Task to run script on startup

```shell
schtasks /create /tn "Start AutoHotkey script SpaceToUnderscore" /tr 'C:\Program Files\AutoHotkey\AutoHotkey C:\Tools\SpaceToUnderscore.ahk' /sc onstart /RL HIGHEST
```