# Changelog

All notable changes to Ninja Gaiden II Master Edition are listed here. Versions follow [Semantic Versioning](https://semver.org).

## [1.1.1] - 2026-11-20

Improved Reduced Input Delay, wall attack aiming, 2x MSAA fixes and an Infinite Ninpo fix.

### Gameplay

- **ME Combat Fixes**: better aim for wall attacks with the Dragon Sword, Vigoorian Flail, Lunar staff and
  Falcon's Talons
  - X off a wall with the stick held now goes where the stick points. Before, the target was picked on the mirrored
    side
  - Falcon's Talons remember the stick direction during the wind-up
  - With the stick released, the attack picks the enemy in front of you as you leave the wall, and closer enemies
    win over far ones

### Performance

- Improved: **Reduced Input Delay**. One frame less delay (about 35 ms down to about 18 ms
  on screen), with frames still at an even pace. On works on most PCs; Max shows each frame a little sooner, but
  needs some performance headroom. Needs Xenia's `framerate_limit = 0` and no FPS cap in RTSS or the graphics
  driver

### Visual

- Fixed: with **Experimental: Native 2x MSAA**, the fade after a death or a chapter load showed an old picture
  (pause menu, title screen)

### Cheats

- Fixed: **Infinite Ninpo** with an empty ninpo gauge now fills the gauge on the first cast. Before, it let you cast
  but the gauge stayed empty

## [1.1.0] - 2026-11-14

Combat fixes, new cheats and visual options, and MASTER OPTIONS as its own title menu item.

### Gameplay

- New: **ME Combat Fixes** replaces Weapon Property Fixes. Fixes combat flaws of the original game: attacks while
  touching a wall or jumping off it aim at the enemy and connect, OTs on enemies lying on the ground connect, several
  moves aim at enemies more reliably, and with Dragon's Claw and Tiger's Fang the Y, Y, Forward+Y launcher lifts Gaja
  properly and its second Y no longer launches dogs. Applies when you load a save.
- Removed: **Weapon Property Fixes** and **Sigma Framedata Backport**.
- Modern Ranged Combat related bug fixed: the Blade of the Archfiend finisher dealt an extra late hit.
- Modern Ranged Combat now works with Ninpo too - aim with right stick!

### Visual

- New: **Smooth Normal Maps**, on by default. Trilinear filtering for normal maps: removes the moving bands on
  surfaces and softens highlights. Works best with Texture LOD Bias 0 (the default). Off keeps the original look.
- **Hi-res Shadows** is now off by default.
- Fixed (always on): the flickering column and spire geometry in chapter 6, and the missing rose window in Mission 4.

### Cheats

- New: **One-Hit Kill**. Any hit that deals damage kills the enemy.
- New: **Instant Charge** (ET and UT charge at once) and **Rich Essence** (every yellow essence pickup gives
  10,000). Ported from bader0418's Xenia patches.
- Reworked: **Infinite HP**. Ryu takes no damage at any upgrade level, and turning it off no longer leaves the health
  bar at its full-upgrade length.
- Fixed: **Infinite Ninpo** now lets you cast ninpo even when the ninpo gauge is empty, for example at the very
  start of the game.

### Menu

- MASTER OPTIONS is now its own item in the title menu, no longer opened through Options.

## [1.0.3 Hotfix 2] - 2026-10-31

Fixes for Lunar XY Launcher:

- The air combo XXY no longer drifts Ryu forward with every air hit.
- XY and >YY launchers no longer throw enemies too high.
- Lunar XY Launcher no longer changes aerial XX combo.

Also:

- Fixed: All Weapons and Ninpo at Lv1 removed the Dragon Sword from the inventory.

## [1.0.3 Hotfix 1] - 2026-10-30

- Fixed: Weapon Appearance. With a look different from the weapon's level, blood didn't build up on the blade.
- Fixed: with Modern Ranged Combat, the Blade of the Archfiend combo X, X, X, X, Y left Ryu stuck in the air.

## [1.0.3] - 2026-10-30

Fixes and new Visual options.

- Fixed: with Modern Ranged Combat, holding RT charges the bow's Ultimate Technique again, like in the original game.
- Fixed: wrong ambient sounds in some places, for example the fountain in chapter 5 (every 1.0.x release).
- Fixed: Muramasa's shop controls (B closes the shop, RT switches to the Blacksmith, Block on LB no longer switches the shop tabs).
- The game's camera speed sliders now work with Modern Camera.
- New in MASTER OPTIONS > Visual: Hide Ranged on Back (the bow and the Gatling Speargun are not shown on Ryu's back; co-created with [MegidoKira](https://github.com/MegidoKira)).
- New in MASTER OPTIONS > Visual: Weapon Appearance submenu (the look of each melee weapon, Lv1 / Lv2 / Lv3, or one look for all with All Weapons).
- The HUD and menu smoothing from 1.0.2 is now a toggle: Smooth HUD and Menus in MASTER OPTIONS > Visual, off by default.
- MASTER OPTIONS lists now wrap around.

## [1.0.2 Hotfix 1] - 2026-10-25

- Fixed: Vigoorian Flail air Y chain with Modern Ranged Combat.

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
