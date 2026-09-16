# Changelog

## v1.1.1 — Enemy Skins Release and Visual Polish

- Renamed the mod from **Enemy Appearance Variety** to **Enemy Skins** to align with the Player Skins project.
- Retained the stable package ID `cmz.enemy-appearance-variety` so existing installations update in place instead of creating a duplicate mod.
- Expanded and curated the catalog to **989 custom recipes** while keeping authentic default appearances available in every enemy pool.
- Balanced all seven Zombie environment/progression pools at **77 custom recipes each**.
- Retained **196 Skeleton-family**, **46 Felguard/Hell Lord**, and **169 Dragon** custom appearances.
- Rebuilt the Alien catalog around the authentic stock design: stock is the canonical Blue-family body, seven custom canonical body families are used, and **39 custom Alien combinations** are approved.
- Added one tuned native accent relationship per custom Alien body while keeping compatible contrasting accents and rejecting same/unapproved near-neighbor pairings.
- Preserved the stock-derived Alien technology/accent footprint and exact stock cyan fallback behavior.
- Uses persistent stochastic skin selection rather than a shuffle deck or fixed rotation.
- Keeps exact-appearance cooldowns, soft source/family recency penalties, usage/age balancing, and starvation protection so all approved appearances remain reachable without creating a predictable sequence.
- Preserves native loaded-source resolution by default and never upscales lower-resolution sources.
- Keeps runtime scope cosmetic-only: no enemy stats, spawn rules, attacks, animation, model geometry, hitboxes, saves, packets, or game RNG are intentionally modified.
- Completed Windows builder validation and successful in-game visual play testing of the release-equivalent runtime.
- Final metadata-only release hardening removed provisional Rev18 wording without altering runtime C# code or skin-selection behavior.
- Current final builder passes **80 portable contract tests**, source/catalog validation, and **78 reviewed SHA-256 pins**.
- v1.1.1 is distributed under the **AnlionGamer Community Distribution Terms v1.0**.
