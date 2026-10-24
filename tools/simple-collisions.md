# Simple Collisions

Draws a quick collision approximation over the objects placed in the scene you
are editing.

It is an approximation, not the game's collision: each object's own SDK model,
drawn translucent, with its scale made uniform to its X axis. An object scaled
(10, 20, 20) is drawn as if scaled (10, 10, 10).

## Needs

Nothing but the Portal SDK (Godot 4.6). High Poly is optional; with it, Isolate
selected also hides High Poly's model.

## Using it

The **Simple Collisions** panel has:

- **Show simple collisions**: the preview on or off for the current scene.
- **Selected objects only**: only the selected objects, including objects in a
  selected group.
- **Isolate selected**: hides the selected objects' models, leaving their
  collision preview.
- **Color** and **Alpha**: the tint of every preview.
- A status line with how many objects are drawn, and which were skipped and
  why.

These settings are not saved between editor sessions.

## Install

In the Toolbox dock, find **Simple Collisions** and press **Add**. By hand: copy
`addons/bf6_simple_collisions` into your project's `addons` folder and enable
**BF6 Simple Collisions**.
