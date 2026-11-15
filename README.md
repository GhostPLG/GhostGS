# GhostGS

GhostGS is a Fortnite gameserver based on [Erbium](https://github.com/plooshi/Erbium), using upstream commit `f59521dbc3ea53cbee3d74e31f7967007d207ba0`.

This fork retains Erbium's GPL-3.0 license and upstream notices. Credit to plooshi and the Erbium contributors; credit to Milxnor for the Finder code noted upstream.

Each push to `main` builds the x64 server and client DLLs and publishes them as a new [GitHub Release](https://github.com/GhostPLG/GhostGS/releases).

[**Join our Discord!**](https://discord.gg/WxNEGBxfKq)

## Features
- **Version support**: Erbium supports version 3.4 (season 3) to 19.40 (chapter 3 season 1).
> Erbium also has partial support for 1.7.2 (season 0) to 3.3 (season 3) & 20.00 (chapter 3 season 2) to 30.00 (chapter 5 season 3)
- **Easy to use**: Erbium is designed to be fast & easy to configure for new users.

## To-do
- **Creative**
- **XP**
- **Quests**

## Configuration
- In order to change options, go to Erbium/Public/Configuration.h & configure to your liking!

## GhostBackend integration
- When using the matching GhostBackend, run the backend and gameserver on the same machine at `127.0.0.1:3551`.
- The gameserver reads the player's Athena loadout (outfit, backpack, pickaxe, glider, and contrail) and daily quests through the backend's loopback-only internal API, then reports daily quest progress back to the profile.
- Use the **Logs** tab in the GS window to inspect recent integration diagnostics or copy them to the clipboard.
- Do not forward `/fortnite/api/internal/gs/` through a public reverse proxy.

> If you have issues with a specific version or find a bug, please make an issue.

> Contributions are highly appreciated!

> If you use Erbium-derived code, please give the upstream project credit.
> Credit to Milxnor for parts of Finders.cpp.
