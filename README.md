# CastleMiner Z — Enemy Skins

A client-side cosmetic enemy skin mod for **CastleMiner Z 1.9.9.8** that expands visual variety across Zombies, Skeletons, Felguards/Hell Lords, Aliens, and all five Dragon families while preserving the base game's models, animations, gameplay behavior, saves, and multiplayer protocol.

> **Unofficial community project:** Enemy Skins is independently created and published by AnlionGamer. It is not an official CastleMiner Z release and is not affiliated with, sponsored by, approved by, or endorsed by the game's developers or publisher.

**Publisher:** AnlionGamer  
**Current release:** v1.1.1  
**Mod ID:** `cmz.enemy-appearance-variety`

The legacy Mod ID is intentionally retained so v1.1.1 updates prior **Enemy Appearance Variety** installations instead of installing as a second mod.

## Features

- **989 curated custom enemy skin recipes** plus authentic default appearances in every selection pool.
- **539 Zombie skins** across seven balanced progression/environment pools, 77 per pool.
- **196 Skeleton-family skins** with coordinated bone regions and independent weathering.
- **46 Felguard/Hell Lord skins**.
- **39 custom Alien combinations** built around the stock Alien's material language, plus the authentic stock Alien.
- **169 Dragon skins** across Fire, Forest, Lizard/Sand, Ice, and Skeleton Dragons.
- Persistent stochastic skin selection with exact-appearance cooldowns, soft source/family recency penalties, usage/age balancing, and starvation protection.
- No complete-deck rotation and no fixed skin sequence.
- Native-resolution texture generation by default; lower-resolution sources are never upscaled.
- Client-local cosmetic rendering only: no enemy stat, spawn, hitbox, model, save, packet, or game-RNG changes.

## Alien Redesign

v1.1.1 uses the authentic stock Alien as the canonical Blue-family body rather than generating redundant blue recolors.

Seven custom body families are provided:

- Cyan
- Teal
- Green
- Violet
- Crimson
- Amber/Gold
- Icy

Each custom body has one tuned native accent relationship modeled after the stock Alien's dark metallic shell and brighter related technology color, plus compatible contrasting accents. Same-color and unapproved near-neighbor combinations remain excluded. Accent recoloring stays on the stock-derived technology footprint, and Alien emissive color follows the selected appearance while vanilla fallback restores stock cyan.

## Selection and Distribution

Enemy Skins does **not** rotate through appearances in a fixed order and does not force a complete catalog pass before allowing repeats.

Each new enemy receives a persistent stochastic appearance assignment. The selector combines:

- hard cooldowns for recently used exact appearances,
- soft penalties for recently used source/material families,
- usage balancing,
- age bonuses for appearances not seen recently,
- and starvation protection so every approved appearance remains reachable over time.

Authentic default appearances remain first-class candidates in every supported enemy pool.

## Texture Settings

The mod exposes optional texture-detail caps for ground enemies, Skeletons, Aliens, and Dragons.

- **native** follows the texture resolution loaded by CastleMiner Z and is the default.
- **256 / 512 / 1024** act only as maximum caps.
- Lower-resolution game sources are never upscaled.
- The generated texture cache defaults to **192 MiB** and can be adjusted if memory pressure requires it.

## Requirements

- CastleMiner Z **1.9.9.8** (Steam)
- CMZ Mod Manager **1.2.0 or newer**
- CMZ Mod Framework/API **1.0.0 or newer**
- Windows / x86 game process

## Installation

1. Download `CMZ_Enemy_Skins_v1.1.1.cmzmod` from the GitHub Releases page.
2. Install it through CMZ Mod Manager.
3. Enable **Enemy Skins** in the active profile.
4. Adjust the optional texture-detail/cache settings if desired.
5. Launch CastleMiner Z through the Mod Manager.

Installing v1.1.1 updates the existing `cmz.enemy-appearance-variety` mod identity rather than creating a duplicate installation.

## Multiplayer

Enemy Skins is designed as a **client-side cosmetic mod**.

The mod does not add custom multiplayer messages, modify CastleMiner Z's network protocol, or require other players to install Enemy Skins, CMZ Mod Manager, or the CMZ Mod Framework.

Enemy appearance choices are generated and displayed locally by the modded client. Vanilla clients remain compatible.

## v1.1.1 Validation Status

The v1.1.1 runtime and catalog have passed automated validation covering:

- **989** unique-per-pool custom recipes,
- balanced seven-zone Zombie pools,
- all approved default/custom candidates remaining reachable,
- persistent stochastic anti-repeat selection without complete-deck rotation,
- selector state persistence and cache eviction behavior,
- Rev18 Alien body/accent compatibility and native-accent rules,
- exact vanilla Alien stock behavior and cyan fallback,
- native-resolution/no-upscale contracts,
- cosmetic-only patch scope,
- package identity and rename compatibility,
- and reviewed source/document/reference integrity pins.

The current final builder passes **80 portable contract tests**, source/catalog validation, and **78 reviewed SHA-256 pins**. The Windows build path and live CastleMiner Z visual behavior were also play-tested successfully before the final metadata-only release-note cleanup; that cleanup does not alter runtime C# code or skin-selection behavior.

## Privacy

- No telemetry or analytics.
- No web requests or data uploads.
- No custom multiplayer traffic.
- No intentional modification of save data or world progression.
- No game asset redistribution in this repository.

## Save / Removal Safety

Enemy Skins does not intentionally modify world data, progression, inventories, enemy stats, spawn rules, or save formats. Disable or remove it through CMZ Mod Manager. Existing saves are not expected to require conversion.

## Repository Policy

This repository is for **public releases and finished public-facing states only**. Development builders, intermediate test builds, dependencies, diagnostics, extracted game assets, and private build artifacts are intentionally excluded.

The reference manifest for each public release is kept under `Release/`. Installable `.cmzmod` packages and official portable builder ZIPs belong on the GitHub **Releases** page rather than in the repository tree.

## License and Attribution

Enemy Skins **v1.1.1 and the current repository state** are governed by the **AnlionGamer Community Distribution Terms v1.0**. See [`LICENSE`](LICENSE).

The terms allow normal use, source inspection where source is published, and private modification. Public redistribution of the original project, packaged mod, forks, or modified builds requires **prior permission from AnlionGamer** and must remain **non-commercial**. Sale and paid access are prohibited without separate permission.

The original Enemy Skins / Enemy Appearance Variety mod concept, design direction, and release are credited to **AnlionGamer**. Additional attribution and the CastleMiner Z rights notice are documented in [`NOTICE.md`](NOTICE.md).

CastleMiner Z and its original game assets remain the property of their respective rights holders. This is an independent, unofficial fan-made mod project and is not affiliated with or endorsed by the game's rights holders.
