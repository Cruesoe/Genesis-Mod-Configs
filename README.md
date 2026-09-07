# Genesis Mod Configs

A Modlist Configurator preset, same mechanism as ferny's Mod Configs, but holding Cruesoe's own settings for the mods installed alongside the Genesis suite.

## How this works

[Modlist Configurator](https://steamcommunity.com/sharedfiles/filedetails/?id=3009304695) applies the per-mod settings files found in this mod's `Settings/` folder to the player's live RimWorld config on startup. Each file is just a normal mod's own settings XML/JSON, named `Mod_<workshopId>_<ClassName>.xml` (or `.json`).

## Adding a mod's settings to this preset

1. In-game, configure the target mod's settings the way you want them baked into the pack.
2. Use Modlist Configurator's own export feature (see its mod options) to export that mod's current settings file.
3. Drop the exported file into this repo's `Settings/` folder.
4. Deploy and commit.

There's no code to write here — this mod is just a curated collection of exported settings files plus the `Defs/Preset.xml` declaration that tells Modlist Configurator this is a preset.
