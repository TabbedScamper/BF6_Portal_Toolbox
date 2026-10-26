# Bot Navigation (beta)

See where the game's bots can go on the open map, and what soldier bots will do
on yours. The navigation is read from your own Battlefield 6 install through
High Poly, and rebuilt under the objects you place as you edit.

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
- **White post**: a spawner with no navigation within 1.5 m.
- **Cyan line**: select two nodes, for example a spawner and then a capture
  point, to see the way a bot goes from the first to the second. When there is
  no way there, the panel says how far short bots get.

## What bots do with your objects

- A doorway needs to be about 0.9 m wide; under about 0.76 m it never gets
  navigation, and in between it depends on where it falls on the game's grid.
- Steps up to 0.4 m are walked; slopes up to just under 50 degrees.
- Where the base map ships navigation under your objects, bots do not climb
  onto boxes, hop gaps or drop off ledges your objects make. Placed ladders are
  the exception: bots climb them when both ends have navigation.
- Where the base map ships no navigation at all (for example a map built on the
  extended terrain outside the original play area), the game builds it for your
  whole combat area, and there bots can jump and vault some low obstacles, such
  as sandbags in a window. Those jumps and vaults are not drawn yet.
- Destructible railings block bots completely. Doors do not block bots.

These rules were checked against live bots on 115 test lanes, and the sheet
agreed on 114.

## Install

In the Toolbox dock, find **Bot Navigation** and press **Add**. By hand: copy
`addons/bf6_bot_navigation` from the release zip into your project's `addons`
folder and enable **BF6 Bot Navigation (beta)**.

## Credits

The navigation format notes and the first version of the overlay were sent to
us by a community modder working on the same problem.
