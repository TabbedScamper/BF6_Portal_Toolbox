# Bot Navigation (beta)

See where the game's bots can go on the open map, and what soldier bots will do
on yours. The navigation is read from your own Battlefield 6 install through
High Poly, and rebuilt under the objects you place, and on your custom terrain,
as you edit.

## Needs

High Poly, pointed at your Battlefield 6 install. The Toolbox will not add Bot
Navigation without it.

## Using it

Open a map scene, then tick a layer in the Bot Navigation panel:

- **Soldier**, **Boat**, **Vehicle**, **Helicopter**: the navigation the game
  ships for the map, as see-through sheets. Red lines are jumps, drops and
  vaults; orange edges on the Soldier layer are doorways.
- **Soldier, your map**: the soldier navigation as the game rebuilds it under
  your placed objects when the experience starts. Move, add or delete an object
  and the 16 m squares under it are rebuilt within a second.

On **Soldier, your map**:

- **Green**: bots walk here. **Yellow**: they crouch. **Purple**: they crawl.
- **Orange**: a crouch under about 1.2 m. Bots are let in, but a crouching bot
  can get stuck. Raise the ceiling to 1.2 m or more, or lower it under 1.1 m so
  they crawl.
- **Red**: a platform too small to get any navigation (under about 4 m² of
  floor, not joined to anything bigger). Bots never go there, even with a
  ladder up to it.
- **Grey**: no bot from your AI spawners, spawn points or selected markers can
  get here.
- **White post**: a start more than 5.5 m from any navigation. Bots spawned
  there never move.
- **Cyan line**: select two nodes, for example a spawner and then a capture
  point, to see the way a bot goes from the first to the second. When there is
  no way there, the panel says how far short bots get.

## What bots do with your objects

- A doorway needs to be about 0.9 m wide; under about 0.76 m it never gets
  navigation, and in between it depends on where it falls on the game's grid.
- Steps up to 0.4 m are walked; slopes up to just under 50 degrees.
- Bots do not climb onto boxes, hop gaps or drop off ledges your objects
  make: the game gives your objects no jump, drop or vault links. Placed
  ladders are the exception: bots climb them when both ends have navigation.
- The navigation ends at your combat area's outline. A bot outside it has
  none under it.
- A bot that cannot reach where it is sent walks to the start of the walkable
  patch nearest the target and stops there. It does not push on, and sending
  it again does not help.
- Bots that start off the navigation (for example outside the combat area)
  walk straight at their target instead; when something blocks them they jump
  once, which is how they sometimes get over sandbags. They never try twice.
- Destructible railings block bots completely. Doors do not block bots.

## Custom terrain

If your map has a Terrain3D, the sheet stands on its ground instead of the
base map's, and every square of your combat area is rebuilt on it, as the game
does when the experience loads. Terrain edits are picked up as you make them.
A large map takes about ten seconds the first time. In the game, bots ordered
in the first minute of a match can still be on the base map's old navigation
while the game rebuilds it. Needs High Poly 3.2.0.

These rules were checked against live bots on 115 test lanes, and the sheet
agreed on 114. On a community Caspian Border map built on Portal Ocean's custom
terrain, the sheet lay on average within 0.1 m of the navigation the game
built, and every test bot's route matched.

## Install

In the Toolbox dock, find **Bot Navigation** and press **Add**. By hand: copy
`addons/bf6_bot_navigation` from the release zip into your project's `addons`
folder and enable **BF6 Bot Navigation (beta)**.

## Credits

The navigation format notes and the first version of the overlay were sent to
us by a community modder working on the same problem.
