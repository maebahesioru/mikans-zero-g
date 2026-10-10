# Mikan's Zero-G

Mikan the cat is floating in orbit, and there are 15 stars to grab. Also asteroids. Sorry, Mikan.

This is my project for Stardance. It's one file, no images, no libraries, no build step — every cat, star and rock is drawn with plain canvas code.

## How to play

Arrow keys or WASD to thrust. Remember it's zero-g: you don't stop when you let go, you drift. That's most of the game, honestly — learning to aim your drift, grab stars, and not kiss an asteroid. You get 3 hits before Mikan is too dizzy to continue. Grab all 15 stars and you win.

Press SPACE to launch.

## What's actually in it

- **Drift physics.** Thrust adds to your velocity, drag slowly pulls it back down, and the walls bounce you back in. Tuning this was the hardest part of the whole project. My first version felt like ice-skating in syrup, then like a pinball machine — I ended up cutting the thrust power, raising the drag, and softening the wall bounce, and only then did it feel like space.
- **Everything is shapes.** The cat, stars, asteroids and the background starfield are all canvas rectangles and dots. No image files at all. The starfield is just scattered dots that shift a little as you move, so the empty space feels like it's going somewhere.
- **Asteroids** spawn from the edges and cross the screen at random speeds, so no two runs are the same.
- **Sound is math.** The bleeps are WebAudio oscillators — a rising sine when you catch a star, a low sawtooth buzz when you get hit. No audio files, just frequencies.
- **The cat is my character** I keep building things with: she started as a desktop pet, then learned to fit inside a single URL, then got her own corner of the web. A space program felt like the obvious next career move for her.

## Run it

Open `index.html` in a browser. That's the whole setup.

If you want to serve it:

```bash
python3 -m http.server 3843
```

## Files

- `index.html` — the entire game (HTML, CSS and JS in one file, ~260 lines)

## Devlog

The build was logged in the Stardance devlogs — day 1 was the game loop, drift physics and asteroid dodging, and the last session added the procedural starfield and the WebAudio bleeps.
