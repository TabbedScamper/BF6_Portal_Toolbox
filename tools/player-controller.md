# Player Controller

Walk a map in first person from any soldier or loot spawner, as the soldier who
stands there and holding their loadout. The soldier, their eye height, arms,
weapon and movement come from your install through High Poly.

## Needs

High Poly, pointed at your Battlefield 6 install. The Toolbox will not add
Player Controller without it.

## Using it

- **Play from the camera** starts you where the editor camera is, as a default
  soldier. When you stop, the editor camera stays where you walked to.
- The panel lists the open map's soldier and loot spawners; the one selected in
  the scene tree is picked first. **Walk from this spawner** stands you there
  as that soldier.
- WASD walks, Shift runs, Ctrl crouches, Space jumps, Esc stops and returns the
  camera.
- Walk up to a vehicle and press E to drive it.
- **Walk** on the BF6 radial menu does the same as the panel.

## Install

In the Toolbox dock, find **Player Controller** and press **Add**. By hand: copy
`addons/bf6_player_controller` from the release zip into your project's
`addons` folder and enable **BF6 Player Controller**.
