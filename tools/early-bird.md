# Early Bird

Your game has maps the Portal SDK does not ship level scenes for yet. Early Bird
builds those scenes from your install, in the same shape as the ones the SDK
ships, so the map opens in the editor like any other.

## Needs

High Poly, pointed at your Battlefield 6 install.

## Using it

The **Early Bird Maps** panel lists every map your install has that the SDK
does not. A map added by a later game update shows up on its own.

- **Install** builds the map in a separate Godot process (a couple of minutes;
  the editor stays usable), adds it to the SDK's map list and regenerates the
  Object Library with its objects. BF6 Home, Game Mode Setup, High Poly and
  Player Controller then treat it like a shipped map.
- **Remove** takes all of it back out.
- **Trace**: with it on, click the orange blockout geometry and the status line
  names the piece of the level it stands for.

## Install

In the Toolbox dock, find **Early Bird** and press **Add**. By hand: copy
`addons/bf6_early_bird` into your project's `addons` folder and enable
**BF6 Early Bird Maps**.
