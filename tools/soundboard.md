# Soundboard

Every Portal sound, listed by the exact name the Portal SDK and its scripting
use, with search, filters and a waveform for each. Hear a sound, copy the script
line that plays it, or place the SDK's sound scene in your map.

Sounds play from your own install through High Poly. The plugin holds only
names and metadata: no audio ships with it, and nothing is downloaded.

## Needs

High Poly, pointed at your Battlefield 6 install. The Toolbox will not add the
Soundboard without it.

## Using it

- **Search** matches names and tags, with synonyms and typo tolerance. Chips
  narrow by category, 2D/3D/loop and tags; length, pitch, loudness and the
  other measurements take a range.
- **Portal** lists the sounds Portal scripting can play; **Game** lists every
  other sound in your install.
- **Play** plays the sound from your install. The waveform under each card is
  drawn from that audio.
- **Copy code** puts the TypeScript line (`mod.PlaySound(...)`) on the
  clipboard.
- **Place** adds the SDK's sound scene for that sound five metres in front of
  the editor camera, and selects it.
- Announcer voice-over is listed but cannot be played yet.

The first start reads the install's sound list (about a minute). The list and
the waveforms you have seen are cached and reused until the game updates.

## Install

In the Toolbox dock, find **Soundboard** and press **Add**. By hand: copy
`addons/bf6_soundboard` into your project's `addons` folder and enable
**BF6 Soundboard**.
