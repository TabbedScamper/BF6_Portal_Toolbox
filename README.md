# BF6 Portal Toolbox

Editor tools for the Battlefield 6 Portal SDK (Godot). Each tool is a separate
Godot plugin. All of them share one **Toolbox** dock, which lists what you have
installed, shows when an update is out and what changed, and adds the other
tools with one press.

Most tools work through **High Poly**, which reads models, terrain, sound and
layouts from your own Battlefield 6 install while you edit. Nothing from the
game is hosted here or downloaded by the tools. Everything they show comes from
the copy of the game on your machine.

## Tools

| Tool | What it does | Needs |
|---|---|---|
| [High Poly](tools/high-poly.md) | Shows the real models, textures, terrain, water, lighting and the map's own objects in the editor while you build on the SDK's low-poly stand-ins. Preview only: your saved map is unchanged. | Battlefield 6 installed |
| [Player Controller](tools/player-controller.md) | Walk the map in first person from any spawner, as the soldier who stands there, holding their loadout. | High Poly |
| [Soundboard](tools/soundboard.md) | Every Portal sound by its exact SDK name, with search, filters and waveforms. Hear it, copy the script line that plays it, or place it. | High Poly |
| [Early Bird](tools/early-bird.md) | Installs maps your game has that the SDK does not ship yet, as SDK level scenes with their objects in the Object Library. | High Poly |
| [Game Mode Setup](tools/game-mode-setup.md) | Builds a map's official game mode layouts (Conquest, Breakthrough, Rush and the rest) as editable Portal objects. | High Poly |
| [Bot Navigation](tools/bot-navigation.md) (beta) | Where bots can go on your map: the navigation rebuilt under your objects as you edit, where bots walk, crouch and crawl, what they cannot reach, and the route between two points. | High Poly |
| [Extended Terrain](tools/extended-terrain.md) | Shows the ground outside the playable area and the distant landscape around it. | High Poly |
| [Simple Collisions](tools/simple-collisions.md) | Draws a quick collision approximation over placed objects. | Nothing else |

In development, and shown greyed out in the Toolbox until they are ready: BF6
Home, Changes, Game Log, Experience, Blockly, Portal Connect, Extended
Workspace, Prop Organizer, UI Editor, TypeScript Editor, BF2 Importer and
BF2042 Terrain.

## Install

1. Download a tool from [Releases](../../releases). Start with
   **High Poly** if you want the tools that need it.
2. Unzip it into your Portal SDK Godot project folder, so its folder lands in
   `addons/`.
3. Open the project and enable the plugin under
   **Project > Project Settings > Plugins**.

The Toolbox dock comes with every tool. From then on, add and update the others
from there. When several tools have updates, press **Update** on each of them
before you restart the editor: they share the Toolbox's files, so they update
together.

## Updating from High Poly 2.10

High Poly 2.10.0 updates itself to the current 3.x through its own **Check for
updates** button: it takes a small bridge release first, then 3.x with the
Toolbox. Restart the editor when it asks. 3.0.0 updates straight to the new
version, from the Toolbox or High Poly's own button.

## Requirements

- The Battlefield Portal SDK (its Godot editor, 4.6).
- Windows.
- For every tool except Simple Collisions: Battlefield 6 installed (Steam or
  EA app), with High Poly pointed at it.

## License

MIT, see [LICENSE](LICENSE). Bundled third-party software keeps its own licence;
see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

This is a community project. It is not made, endorsed or supported by
Electronic Arts or Battlefield Studios. Battlefield is a trademark of
Electronic Arts Inc.
