# Game Mode Setup

Builds a map's official game mode layouts as editable Portal objects: capture
points, sectors, HQs, spawns, vehicles, M-COMs and the volumes that go with
them. Conquest, Breakthrough, Rush, Domination, Escalation, King of the Hill,
Operations, Obliteration, Sabotage, Strikepoint, the deathmatch modes, and
Carrier Strike, Gauntlet and Payload where a map has them.

Layouts are read from your install through High Poly, so a game update is
picked up the next time you open the list.

## Needs

High Poly, pointed at your Battlefield 6 install.

## Using it

1. Open a map scene.
2. Open the **Game mode** list. It shows the modes your install has for that
   map; hover one for how its objectives work.
3. Pick one. The layout is built as a node in your scene and selected. Save the
   scene when you are happy with it.

Also in the panel:

- **Swap Team 1 / Team 2** swaps HQ ownership, faction vehicles, objective IDs
  and team spawns for the built layout. Press again to swap back.
- **Andys Template Addons** adds Andy's TeamSwitcher, AI Spawns and
  EndGameCamera template objects.
- Vehicle and emplacement spawners show the SDK vehicle they spawn, and High
  Poly draws the real vehicle over it. Editor only: the saved scene keeps just
  the spawner.
- **Clear cached layouts** deletes the layouts read so far. Nodes already in
  your scene are not touched.

Rush and Breakthrough carry the map's exact sector, objective and HQ links.
Where those links cannot be resolved for a map, the panel says so instead of
guessing.

## Install

In the Toolbox dock, find **Game Mode Setup** and press **Add**. By hand: copy
`addons/bf6_gamemode_setup` into your project's `addons` folder and enable
**BF6 Game Mode Setup**.
