# Changelog

All notable changes to Ninja Gaiden II Master Edition are listed here. Versions follow [Semantic Versioning](https://semver.org).

## [1.0.2] - 2026-10-24

Visual update and fixes.

- New in MASTER OPTIONS > Visual: Texture LOD Bias (0 / -1.0 / -1.5, default 0 removes the floor and texture shimmer at Xenia scale 2x), Hi-res Shadows (always the 1024 shadow map, on by default), Skip 4x MSAA Clear (10-15% less GPU load, same picture, on by default).
- HUD and menu sprites are now filtered: no more pixel steps at Xenia scale 2x.
- New optional patches, off by default: Hi-Res Font (sharp UI text at Xenia scale 2x) and Experimental: Native 2x MSAA (16:9 only).
- MASTER OPTIONS now shows in every game language (title menu and pause screen).
- 21:9: the screen no longer goes black during Ryu's death slow motion.
- No Post-Effects keeps the death blur.
- Infinite Ninpo: the ninpo icons on the HUD burn and refill correctly.
- Free camera in special moves: no more camera pulse during OTs.
- Ryu Fuse: a stuck Incendiary Shuriken no longer plays the explosion sound on contact, only when it explodes.
- Removed the leftover "Master Menu" entry from the title Options screen.

## [1.0.1] - 2026-10-23

Bug fixes.

- Fixed Eclipse Scythe and related crash
- Fixed Modern Camera related crashes (especially Chapter 13).
- 21:9: the New Game+ confirmation and GAME OVER screens now align properly.
- Removed Auto-Skip All Cutscenes: could crash the game. This will be fixed in future updates.

## [1.0.0] - 2026-10-22

First release.

- In-game MASTER OPTIONS menu (title menu and pause menu) with all options Off by default.
- Modern Camera, Modern Ranged Combat (bow, shuriken on B, Gatling Speargun under water), Sigma Reticle.
- Weapon & Movement Tweaks: Sigma Framedata Backport, Weapon Property Fixes, Lunar XY Launcher, IS fixes.
- Quality of Life, Visual Options (including No Post-Effects with cutscene heat haze), Cheat Menu.
- Reduced Input Delay (Off / -1 / Max), 1280x720 on by default, 21:9 ultrawide in the patch list.
- Works with ISO, GOD and unpacked game folders; the mod files live in Xenia's plugin folder.
