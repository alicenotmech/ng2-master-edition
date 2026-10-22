# NINJA GAIDEN II — Master Edition

![Ninja Gaiden II Master Edition](images/banner.jpg)

Mod-menu with bunch of features for the original **Ninja Gaiden II** on the **Xenia Edge** emulator.

## What you get

- **In-Game Mod Menu**: MASTER OPTIONS, with a bunch of toggles that work right in the game
- **Modern Camera**: a reworked, free and more comfortable camera, backported from the modern versions of
  Ninja Gaiden II
- **Modern Ranged Combat**: Sigma 2 ranged weapon controls, even for Gatling Speargun. Now shuriken is ALWAYS B!
- **Weapon & Movement Tweaks**
  - **Sigma Framedata Backport**: small frame data tweaks from the modern versions of the game, mostly
    smoother and more responsive transitions between Ryu's moves
  - **Weapon Property Fixes**: a port of Fiend Busa's mod for more precise tracking on several weapons
- **Quality of Life**: skip the death screen, skip cutscenes, reduced input delay, consistent 60 fps
  cutscenes, a HUD that fades out when you're not fighting, and more
- **Visual Options**: less bloom, no blur effects, MORE BLOOD AND GORE!
- **21:9 Ultrawide Support**: in Xenia's patch list
- **Cheat Menu**: all weapons, infinite HP and ninpo, including Freeze Enemies

## What you need

- [Xenia Edge](https://github.com/has207/xenia-edge)
- Your own copy of **Ninja Gaiden II** with **Title Update 3** installed in Xenia

## How to install

0. Backup your .toml patch files from `patches` folder
1. Download `master-edition.zip` from the [latest release](../../releases/latest) and extract it
2. Copy `patches` and `plugins` folders into:
  - Windows: `Documents\Xenia`
  - Windows with portable.txt: directly in folder with `xenia-edge.exe`
  - macOS: `~/.local/share/Xenia` (hidden folder, press **Cmd+Shift+.** in Finder)
  - Linux:  `~/.local/share/Xenia`
3. In Xenia's settings, turn on plugins: `Configuration > General > allow_plugins` or in config `allow_plugins = true`  
4. Start the game. You'll find **MASTER OPTIONS** in the title menu, and in the pause menu

Stability on Linux and macOS is NOT GUARANTED 'cause those builds are still less polished and unstable.

If you already use other patches or plugins for Ninja Gaiden II, make a copy of them first. **Don't mix this mod
with other Ninja Gaiden II patch files!**

## Menu options

Everything starts **Off**, so the game plays exactly like the original until you turn something on.

### Gameplay
- **Modern Ranged Combat** — the shuriken is always on B and gone from the inventory, ranged weapons fire with
  RT. Aim the bow and the Gatling Speargun with LT and the right stick, move and shoot while aiming the bow
- **Sigma Reticle** — the Sigma aiming reticle for the bow and the Gatling Speargun
- **Block on LB** — swaps LT and LB
- **Infinite Ammo** — arrows and shuriken never run out, the ammo counter is hidden
- **Sigma Framedata Backport** — move timing from Sigma 2 and Black: dash into run, water moves, landing transitions. Not affecting gameplay in general, but make controls much responsive.
- **Weapon Property Fixes** — ported from Fiend Busa's
  [Weapon Property Fixes](https://www.nexusmods.com/ninjagaiden2black/mods/100) for Ninja Gaiden 2 Black
  Only the changes that apply to the original game and differ from it are included: tracking on Flail
  Forward Y, Lunar 360 UT, Dual Sword Forward Y, Tonfa Flying Swallow and Flail running X
- **Lunar XY Launcher** — Lunar XY launches enemies, like in Sigma
- **IS Single Shuriken** — IS ninjas throw one Incendiary Shuriken
- **IS Visibility** — less intense Incendiary Shuriken explosions
- **IS Fuse** — the IS ninjas' Incendiary Shuriken stick into walls and explode after a moment, like in the 2008
  prototype
- **Ryu Fuse** — the same for Ryu's Incendiary Shuriken

### Camera
- **Modern Camera** — a free and more comfortable camera, ported from the modern versions of Ninja Gaiden II.
  Applies when you load a save
- **OT/UT Free Camera** — keep camera control during Obliteration Techniques, Ultimate Techniques, throws and
  more
- **No Screen Shake** — no shake on hits, finishers and explosions

### QoL
- **Skip Death Screen** — skips the GAME OVER screen
- **Auto Chapter Screen** — chapter title cards and mission briefings continue without a button press
- **First Time Cutscene Skip** — you can skip any cutscene, even the first time you see it
- **Auto-Skip All Cutscenes** — every cutscene and movie is skipped automatically
- **HUD** — show the HUD, let it fade out when you're not fighting, or hide it
- **Hide Combat Counters** — hides the hit counter, karma and boss health, while health, ninpo and ammo stay.
  A test feature for further experiments with HUD options
- **Reduced Input Delay** — the game normally keeps up to two finished frames waiting before it shows them, and
  that waiting is the delay you feel
  - **-1** lets only one frame wait: about one frame less delay (three frames become two)
  - **Max** lets no frames wait: the lowest delay. The game then waits for your graphics card every frame,
    so it needs a performance headroom, or it may stutter
- **60 FPS Cutscenes** — cutscenes run at a steady 60 fps
- **All Difficulties Unlocked** — Mentor and Master Ninja are available for a New Game

### Visual
- **More Blood** — twice as much blood stays on floors and walls
- **More Blood Particles** — bigger blood spray on every hit and delimb
- **Reduce Bloom** — bloom at half strength, less overexposure
- **No Post-Effects** — no blur, no white flashes

### Cheats
- **Infinite HP**
- **Infinite Ninpo**
- **Freeze Enemies** — enemies stand still
- **All Weapons and Ninpo** — every weapon and ninpo from the start, at Lv1 or Lv3
- **All Crystal Skulls** — all 30 crystal skulls count as collected
- **Max HP and Ninpo** — full health and ninpo upgrades from the start

Cheats that give items or upgrades stay in your save if you save the game at a statue

## Good to know

- Most options work right away. **Modern Ranged Combat** and **Modern Camera** kick in the next time you load a
  save. If you change them during play, the menu reminds you with "Reload required"
- **1280x720** is on by default: the game renders at 1280x720 instead of its native 1120x584
- **Widescreen 21:9** is in the same patch file, switched off. For a 3440x1440 picture, also set Xenia's
  resolution scale to 2

## Known Issues

- **Xenia restart crash** — restarting the game in the same Xenia window can cause a crash when loading a save
  **Close Xenia completely before starting again.** This is a bug in Xenia's plugin system, not in the mod
- **60 FPS Cutscenes** — in my experience, audio seems to gradually go out of sync in some cutscenes
  This still needs more testing and research
- **Infinite Ninpo HUD** — charge icons can disappear after using ninpo even though you can still keep casting it

## Credits

alicenotmech — mod author. 1280x720 Resolution patch by Margen67.
Weapon Property Fixes ported from the Ninja Gaiden 2 Black mod by Fiend Busa.
Ninja Gaiden II © KOEI TECMO GAMES / Team NINJA. This is an unofficial fan project.
