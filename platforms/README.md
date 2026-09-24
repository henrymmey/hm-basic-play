# Platform packages

The modpack has separate Packwiz roots for each distribution platform:

- `modrinth/` uses Modrinth metadata and produces `hm-basic-play-<version>.mrpack`.
- `curseforge/` uses CurseForge metadata where a compatible file exists and produces `hm-basic-play-<version>.zip`.

Files without a compatible CurseForge release remain bundled in the CurseForge package.
