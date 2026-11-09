# UI Editor (preview)

Design, animate and hear Portal UI in Godot, then export it as code your mode
script runs. Lay out texts, images and boxes on a 1920 x 1080 canvas, make them
come in, move and react when something happens in your mode, and play it back
with its sounds before you test in the game.

## Needs

Nothing else to design, animate and export. For weapon, gadget and icon
pictures drawn the way the game draws them, the game's sounds and the radio,
also install High Poly (and the Soundboard for sounds) and set your Battlefield
6 folder in High Poly.

## Using it

1. Click **BF6 UI** at the top of the editor, beside 2D, 3D and Script.
2. Pick a **Template...** (whole mode HUDs to start from) or an **Empty
   design**, then click pieces on the canvas and change them on the right.
3. Open **Moments** to make things happen: a moment is something in your mode
   (a kill, a round start), and its steps are what the UI does then. Press
   **Space** to play it.
4. **Save** (Ctrl+S) writes the design and its texts to your mode's project;
   **Export** gives the code your mode script runs.

- **Weapon builder**: a Weapon image's settings open a screen laid out like the
  game's weapon customization. Try attachments slot by slot, save loadouts in
  the design or in your own library, and apply them.
- **Open a mode script** shows an existing mode's UI without starting the game,
  ready to edit.

This is a preview: designs and exports work, and more of Portal's UI calls
are being added.

## Install

In the Toolbox dock, find **UI Editor** and press **Add**. By hand: copy the
`addons` folder from the zip into your project and enable **BF6 UI Editor**.
