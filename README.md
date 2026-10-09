# Mikan's Zero-G 🚀🐱

A tiny zero-gravity game: Mikan the pixel cat is floating in orbit and needs
your help to collect 15 stars — while dodging asteroids.

Made for [Stardance](https://stardance.hackclub.com/) (Hack Club × NASA).

## Play

Open `index.html` in a browser. That's it — single file, no build, no assets.

- **Arrow keys / WASD** — gentle thrust (it's zero-G: you drift!)
- Collect **★ 15 stars** to complete the mission
- Dodge the gray asteroids — 3 hits and the cat is dizzy

Everything is drawn with canvas rectangles and a bit of math: the cat, the
stars, the rocks, the floating starfield, and even the little `bleep`s
(WebAudio oscillators). No images, no libraries.

## Why a cat in space?

Continuity! Mikan started as a desktop pet, learned to fit inside a single
URL, has her own corner of the web — and this is her space program.

## Files

- `index.html` — the whole game (HTML + CSS + JS in one file)

## Run locally

Just open `index.html`. Or:

```bash
python3 -m http.server 3843
```
