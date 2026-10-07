# Starbank

> **This is a fixed version (1.9.1) of [BlueRaja/Starbank](https://github.com/BlueRaja/Starbank).**
> The changes are also proposed to the original project in [BlueRaja/Starbank#23](https://github.com/BlueRaja/Starbank/pull/23).
>
> **Download:** [latest release](https://github.com/Mates31cz/Starbank/releases/latest) – installer (`StarBank.Setup.msi`, replaces an installed StarBank 1.9) or portable ZIP.
>
> **Fixes**
> - Startup no longer gets stuck at *"Initializing map cache"*. Maps that call `BankLoad()` with a variable many times (e.g. *Trancespace Fortress III*) made the original version run for hours at 100% CPU, which got worse as the Battle.net cache collected more map versions.
> - Loading no longer freezes the whole system (limited to 4 threads, below-normal priority).
> - Banks whose keys hold several named values can now be edited, saved and re-signed.
> - Non-ASCII text in map scripts is no longer cut off.
>
> **New features**
> - Map info is cached between runs (`MapCache.dat`), so startup is faster.
> - Bank backups in a `Backups` folder next to the exe (or in `%LOCALAPPDATA%\StarBank` when installed in Program Files): back up all banks (*Tools* menu) or a single map's banks, restore any backup, automatic backup before the first edit, and a `[!]` marker for maps whose banks were never backed up.
> - *Re-sign* button for the currently selected bank.

A graphical editor for Starcraft II custom map save files _(aka "bank files")_.  Supports multiple accounts, protected maps, hidden bank files, and much more.

More information on installing and using Starbank can be found [here](https://web.archive.org/web/20190716174221/http://www.d3scene.com/forum/starcraft-2-custom-maps/67976-starbank-starcraft-ii-bank-file-editor-custom-map-saves-v1-8-a.html).

![Example screenshot](http://i.imgur.com/GNK8ZWp.png)
