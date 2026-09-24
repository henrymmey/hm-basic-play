# HM Basic Play

[![Static Badge](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/henrymmey)
[![Static Badge](https://img.shields.io/badge/Website-henrymeyer.de/gaming-green)](https://henrymeyer.de/gaming)

---

This modpack aims to improve the Vanilla Minecraft experience through small optimizations and tweaks.

It was developed to be compatible with the rules of most common servers. However, it remains your responsibility to verify the permitted mods for each specific server.

---

## Features

- **Small Optimizations:** Built on the latest Fabric loader with essential mods like Sodium, Lithium, and FerriteCore.
- **Quality of Life:** Small enhancements like dynamic crosshairs and better UI handling.
- **Visual Improvements:** Mods like Iris Shaders and 3D Skin Layers for a more modern look.
- **Vanilla-Friendly:** No gameplay changes. It’s the Minecraft you know.

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

# Export for Modrinth
VERSION=26.3-1.1.0
cd platforms/modrinth
packwiz modrinth export -o ../../hm-basic-play-${VERSION}.mrpack

# Export for CurseForge
cd ../curseforge
packwiz curseforge export -o ../../hm-basic-play-${VERSION}.zip
```

### Project Structure

```
platforms/modrinth/    — Modrinth Packwiz root
platforms/curseforge/  — CurseForge Packwiz root
.github/workflows/     — Automated platform-specific release exports
```

## Release

Create a release with proper Tags and Name. Everything should be published automatically.
