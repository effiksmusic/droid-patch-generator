# droid-patch-generator
Advanced Patch Generator scripts for [Der Mann mit der Maschine DROID](https://vpme.de/droid-universal-cv-processor/) Forge based on the existing scrips from [DROID Forge](https://github.com/Zarkuun/droidforge/tree/main/droidforge/pg).

### Advanced Sequencer — what it adds to the stock generator

Same sequencer, fewer limits:

- Option to use E4 encoders instead of M4 motor faders
- more than four tracks, with a second B32 for the extra buttons
- performance menu spread over pages, so every track keeps its entry
- track sections built as clones the Forge keeps in sync
- one set of presets for all tracks, which saves a lot of RAM
- fixed button layout that no longer shifts when features change
 -extra presets: Less RAM and 8 Tracks

### effiksmusic Sequencer — what it adds on top of Advanced

- root note sequencer on the faders of the performance menu, playing root note and scale as a sequence into every track, optionally out via MIDI
- four track algorithmic drum sequencer on a B32 and an E4 of their own
- one melodic track can play four voice chords, with its second fader layer controlling the harmonic shift
- velocity routed per track: CV output, MIDI, or nowhere
- fewer display texts inside the tracks, to save RAM
- the two lucky functions on separate buttons
- a default sequence length that leaves the longer pages reachable

### Installing the script

Copy the file into the Forge's patch generator folder and restart the Forge. The generator then shows up under its own name.

Do not overwrite the generators that ship with the Forge — it rewrites those on every start and your copy would be gone.

Two things to watch for: the generator stops with a message when it runs out of buttons, CV outputs or gates, and the fix is to switch off a feature or add a G8. And a full configuration sits close to the limits of the master, so keep an eye on the size and RAM display in the Forge and turn on compression.
