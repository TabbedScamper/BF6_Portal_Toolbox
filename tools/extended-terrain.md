# Extended Terrain

See the ground outside the playable area, and the distant landscape around it,
for the map you have open. Both are read from your install through High Poly.

## Needs

High Poly, pointed at your Battlefield 6 install. The Toolbox will not add
Extended Terrain without it.

## Using it

Open a map scene, then:

- **Terrain around the map** shows the real ground that surrounds the play
  area. The SDK's flat terrain is hidden while it is on.
- **Distant landscape (backdrop)** shows the skyline and out-of-bounds scenery
  beyond the terrain's edge. It is heavy, so it is off by default.

These are the same layers as High Poly's **Terrain** and **Backdrops**
switches; changing one place changes both. They are a preview only: nothing is
saved into your map or included when you export.

## Upgrading from an earlier version

Earlier versions downloaded terrain into `res://bf6_terrain_pack`. If that
folder is in your project, the panel shows **Remove old downloaded terrain**,
which removes those nodes from the open scene and deletes the folder. Save the
scene afterwards.

## Install

In the Toolbox dock, find **Extended Terrain** and press **Add**. By hand: copy
`addons/bf6_terrain_pack` into your project's `addons` folder and enable
**BF6 Extended Terrain**.
