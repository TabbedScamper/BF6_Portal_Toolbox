# High Poly

Build Portal maps in the SDK's Godot editor while seeing the real map: textured
models, the terrain around the play area, water, the level's lighting and its
original objects, instead of grey stand-ins on a green island.

Everything High Poly adds is an editor-only preview. The SDK's low-poly objects
stay what your scene saves and what the Portal exporter ships; High Poly never
changes them, and your level file is the same with it on or off.

## Needs

- Battlefield 6 installed on the same machine (Steam or EA app). High Poly reads
  it directly and says so before doing anything when it cannot find it.
- The Portal SDK (Godot 4.6), on Windows.

Nothing is downloaded and nothing is hosted. After a game update, the map you
open next is simply read again. The first read of a map takes a minute or so;
after that it comes from a cache on your machine, which High Poly updates keep.

The caching screen (High Poly panel > **Show caching progress**) has a
**Recache** button beside each stage and on every map, to redo just that part
if something looks wrong.

## What it shows

- **Detail Mode**: placed objects as their real textured models, or as the SDK
  ships them ("Low-Poly (what you export)").
- **Terrain**: the real ground and water around the play area, at the in-game
  height. Mesh density is selectable.
- **Backdrops**: the distant skyline and out-of-bounds scenery.
- **Water**: rivers, harbours and sea at the real height.
- **Original map objects**: the level's own buildings, vehicles and props.
- **Prop Lighting** and **Grass**: the lights placed props carry, and the
  ground vegetation around the camera.
- **Lighting** and **Shadows**: the level's sun, sky, fog and exposure.
- **Range**: how far all of the above keeps drawing.

High Poly is also what Player Controller, Soundboard, Early Bird, Game Mode
Setup, Extended Terrain and Bot Navigation read the game through.

## Install

Download `BF6_High_Poly_Godot_Plugin-3.2.1.zip` from
[Releases](../../../releases), unzip it into your Portal SDK project folder,
and enable **BF6 High-Poly Preview** under
**Project > Project Settings > Plugins**. The Toolbox dock comes with it.

## Updating from 2.10

Press **Check for updates** in High Poly 2.10.0. It installs a small bridge
release first, which then installs 3.2.1 together with the Toolbox. Restart the
editor when it asks.
