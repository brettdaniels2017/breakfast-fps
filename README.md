# Brunch Raid

A breakfast-themed first-person shooter in a single HTML page. You pack two weapons, then clear waves of leftovers across an open diner lot, a kitchen deck, and the Salsa Cantina next door.

**Play:** [https://brettdaniels2017.github.io/breakfast-fps/](https://brettdaniels2017.github.io/breakfast-fps/)

## Run it locally

The page loads Three.js from a CDN, so you need a local server (opening the file directly can block modules).

```bash
cd breakfast-fps
python3 -m http.server 8766
```

Then open [http://127.0.0.1:8766/](http://127.0.0.1:8766/).

## How to play

1. Pick **exactly 2** of the 6 weapons.
2. Press **Start brunch raid**. Click the view if the browser asks for pointer lock.
3. Survive waves. After the last leftover dies, the next wave starts in **10 seconds**.
4. If your stomach hits 0, that’s Burnt Toast — change kit and sit again.

### Controls

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Look |
| Space | Jump |
| Click | Fire |
| 1–2 / scroll | Swap the two guns in your kit |
| Shift | Aim (Maple Marksman scope, 2× zoom) |
| R | Reload |
| Esc | Pause (unlocks the mouse) |

## Armory

You only take two of these into a run.

| Weapon | Role |
| --- | --- |
| Toast Launcher | Mid-range slices |
| Bacon Lash | Short grease whip |
| Syrup Shotgun | Close sticky blast |
| Espresso SMG | Fast spray |
| Pancake Frisbee | Thrown stack, heavy hit |
| Maple Marksman | Bolt-action sniper. Shift for a 2× scope. One shot, then a 2s bolt. Unscoped, a gold ring on the crosshair shows that cooldown. |

## Leftovers

Waves mix:

- Hangry Egg
- Rogue Sausage
- Cereal Haunt (floating bowl of loops)
- Avocado Brute
- Waffle Stack
- Coffee Creep

They melee only, path around the lot, and climb stairs. Each wave adds a couple more leftovers. Every 5th wave they get a **20% health buff** (it stacks). The wave after a buff, pack size resets to the starting count.

## Map

- Open diner lot with patio seating
- U-shaped stairs up to the kitchen deck
- Kitchen under the deck, plus a side roof
- **Salsa Cantina** to the left, linked by a second-floor bridge

## Project

Everything lives in `index.html` (markup, CSS, and the game). Three.js r160 loads from unpkg via an import map.

Repo: [brettdaniels2017/breakfast-fps](https://github.com/brettdaniels2017/breakfast-fps)
