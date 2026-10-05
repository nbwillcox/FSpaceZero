# FSpaceZero

A free, retro sci-fi hover racer in chunky pixel art with 8-bit music, a head nod to the classic SNES-era futuristic racers. Strap into one of four anti-gravity machines, hit the dash pads, dodge the mines and fight a pack of 19 rivals through 15 circuits across five alien worlds.

**Play it in your browser:** https://nbwillcox.github.io/FSpaceZero/

Everything is generated in code: the track is a flat texture drawn through a perspective ("Mode-7" style) renderer, all sprites, skies and scenery are pixel art built at startup by a tiny software rasteriser, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceContra](https://github.com/nbwillcox/SpaceContra), [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpaceDug](https://github.com/nbwillcox/SpaceDug), [SpaceFrogger](https://github.com/nbwillcox/SpaceFrogger) and the rest of the Space series, with the same look and feel.

## Controls

| Action | Keyboard | Gamepad |
| --- | --- | --- |
| Steer | `←` `→` or `A` `D` | left stick / d-pad |
| Accelerate | `↑`, `W` or `Z` | `A` or right trigger |
| Brake | `↓` or `S` | left trigger |
| Boost (burns energy) | `X` or `Space` | `X` / `B` / `Y` |
| Side-slide left / right | `Q` / `E` | `LB` / `RB` |
| Pause | `P` or `Esc` | `Start` |

Menus work with the arrow keys and `Enter`, the mouse, or a gamepad.

## Racing

- **Grand Prix:** three cups (Meson, Quasar, Pulsar) of five races each, 20 racers on the grid, 3 laps per race. Finish inside the cut (top 10 / 8 / 6 on Novice / Standard / Expert) to advance. You get 3 machines per cup; points per race decide the cup standings.
- **Time Trial:** any of the 15 tracks, alone on the road, chasing your best lap with a ghost of your fastest lap.
- **Energy:** the power bar is your armour *and* your boost fuel. Rails, mines and shoving rivals drain it, boosting burns it, and the green recharge strip on the road before the finish line refills it. Run out and your machine blows up.
- **Hazards:** dash pads (free speed), ramps (airborne), mines, rough patches (slow), ice (slippery) and recharge strips.
- **Four machines:** VOLT-7 (balanced), MANTIS (fastest, slippery), RHINO (armoured), WISP (grips like glue).
- **Five worlds:** Neon City, Frost Belt, Magma Ring, Spore Jungle and Orbital Station, each with its own look and chiptune theme (the music speeds up on the final lap).
- Best times, best laps, cup results and ghosts are saved in your browser.

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Add `?t=N` (0-14) to the URL to jump straight into a race on that track, with `&m=` for the machine (0-3) and `&d=` for the difficulty (0-2).

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/FSpaceZero

This is an original game inspired by classic racing games. It uses no assets, names or code from any existing game.
