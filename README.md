# HM Basic Play

A client-side Fabric modpack for Minecraft 26.2 focused on performance optimization, quality-of-life improvements, and visual enhancements. Managed with [packwiz](https://packwiz.tools/) and automatically published to [Modrinth](https://modrinth.com/).

## Features

- **Performance** — Sodium, Lithium, Iris, FerriteCore, C2ME, Entity Culling, and more
- **Visuals** — Complementary Reimagined/Unbound shaders, 3D skin layers, custom ore resource packs
- **Quality of Life** — BetterF3, Zoomify, Dynamic Crosshair, Simple Voice Chat, Mod Menu integration
- **Privacy** — No Chat Reports
- **Cross-version support** — ViaFabricPlus

## Installation

Download the latest `.mrpack` from [Modrinth](https://modrinth.com/modpack/kUYTdD3h), then open it with the Modrinth App or any launcher that supports `.mrpack` files.

## Development

### Prerequisites

- [packwiz](https://packwiz.tools/) CLI

### Useful Commands

```sh
# Install a mod from Modrinth
packwiz modrinth add <mod-slug>

# Remove a mod
packwiz remove <mod-slug>

# Update all mods
packwiz update --all

# Export for distribution
packwiz modrinth export -o release.mrpack
```

### Project Structure

```
mods/            — Mod metadata (.pw.toml files)
resourcepacks/   — Resource pack metadata
shaderpacks/     — Shader pack metadata
config/          — Mod configuration files
options.txt      — Default Minecraft client options
```

## Release

Releases are built and published to Modrinth automatically via GitHub Actions when a GitHub Release is published. The workflow exports the pack using `packwiz modrinth export` and uploads the resulting `.mrpack` to Modrinth.
