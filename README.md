# Agent Scramble

A breakfast-themed first-person shooter in a single HTML page. Pack **three** weapons, then clear waves of leftovers across an open diner lot, a kitchen deck, and the Salsa Cantina next door.

**Play:** [https://brettdaniels2017.github.io/breakfast-fps/](https://brettdaniels2017.github.io/breakfast-fps/)

## Run it locally

The page loads Three.js from a CDN, so you need a local server (opening the file directly can block modules).

```bash
cd breakfast-fps
python3 -m http.server 8766
```

Then open [http://127.0.0.1:8766/](http://127.0.0.1:8766/).

## How to play

1. Pick **exactly 3** of the 7 weapons.
2. Press **Start Agent Scramble**. Click the view if the browser asks for pointer lock.
3. Survive waves. After the last leftover dies, the next wave starts in **10 seconds**.
4. If your stomach hits 0, that’s Burnt Toast — change kit and sit again.

### Controls

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Look |
| Space | Jump |
| Click | Fire |
| 1–3 / scroll | Swap the three guns in your kit |
| Shift | Aim (Marksman 2× scope, Link Launcher 1.5× irons) |
| R | Reload |
| Esc | Pause (unlocks the mouse) |

## Armory

You only take three of these into a run.

| Weapon | Role |
| --- | --- |
| Toast Launcher | Mid-range slices |
| Bacon Lash | Short grease whip |
| Syrup Shotgun | Close sticky blast |
| Espresso SMG | Fast spray |
| Pancake Frisbee | Thrown stack, heavy hit |
| Maple Marksman | Bolt-action sniper. Shift for a 2× scope. One shot, then a 2s bolt. Unscoped, a gold ring on the crosshair shows that cooldown. |
| Link Launcher | Sausage rockets with splash. Shift for 1.5× iron sights. Slow fire, 3s reload. |

## Leftovers

Waves mix:

- Hangry Egg
- Rogue Sausage
- Cereal Haunt (floating bowl of loops)
- Watermelon Brute
- Waffle Stack
- Coffee Creep

They melee only, path around the lot, and climb stairs. Wave 1 starts with 8 leftovers. Each later wave in a 5-round cycle is **+50%** of the last pack. Every 5th wave they also get a **20% health buff** (it stacks). After a buff, pack size resets to 8.

## Map

- Open diner lot with patio seating, ringed by trees and an unpassable bush wall
- U-shaped stairs up to the kitchen deck
- Kitchen under the deck, plus a side roof
- **Salsa Cantina** to the left, with a bar, tables, and a second-floor bridge

## Project

Everything lives in `index.html` (markup, CSS, and the game). Three.js r160 loads from unpkg via an import map.

Repo: [brettdaniels2017/breakfast-fps](https://github.com/brettdaniels2017/breakfast-fps)

## Goals

Still a single-file breakfast raid, with a few bigger slices in mind:

- **Modes** — keep the current wave survival as the default, then add timed rushes, a high-score endless scramble, and a quieter kit-test range.
- **Maps** — more lots besides the diner/cantina block: a night market, a rooftop brunch, maybe a food-truck yard, each with its own routes and sightlines.
