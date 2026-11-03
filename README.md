# BLOOP — a Claude Opus 5.5 button

*The button that wants to be pressed.*

One button. It's a living blob of liquid matter, rendered in real time by a custom WebGL metaball shader.

**Open `index.html` in any modern browser.** It's a single file with no dependencies and no build step, and it works on desktop and mobile.

## What it does

- **It wants you.** It breathes, hops when it's bored, and stretches out a gooey pseudopod toward your cursor.
- **Press:** your finger dents the jelly with a deep, soft *thock* and a haptic tick.
- **Release:** it springs back, ripples spread across the surface, and droplets splash out. Then the droplets get pulled home and merge back in, each one making a little *plip* on a pentatonic scale.
- **Every click is a note.** Clicks climb through a chord progression, so clicking fast plays a song.
- **Combos:** fast clicking builds a ×combo (*nice → juicy → delicious → unstoppable…*), and the floor grid starts pulsing to the rhythm.
- **Press and hold:** it fills with pressure. It inflates, trembles and glows over a rising synth riser. Let go and it detonates: a shockwave bends the floor, the screen shakes, a bass boom hits, and you get up to +10 presses.
- **It evolves.** Milestones make the blob tear itself into an orbiting ring and re-form as new matter, with a new key and a new instrument:
  I Gummy → II Mercury → III Slime → IV Magma → V Gold → VI Prism → VII Nebula → VIII Singularity (a black hole that gravitationally lenses the floor) → loop.
- The ring around the button shows progress to the next (secret) form. Progress is saved locally.

## Details

- All audio is synthesized with the Web Audio API (FM bells, glass partials, filtered saws, generated reverb). It starts only after the first interaction. Press **M** or use the corner button to mute.
- Keyboard: focus the button and hold **Space** / **Enter**. Holding to charge works from the keyboard too.
- Multi-touch: a second finger counts as an extra tap.
- Adaptive resolution keeps the frame rate smooth on weaker GPUs. There's a Canvas2D fallback if WebGL is unavailable, and `prefers-reduced-motion` disables screen shake.
- `index.html?reset` clears saved progress.
