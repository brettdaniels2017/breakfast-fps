# Agent Scramble

**[Promo](https://brettdaniels2017.github.io/breakfast-fps/)** · **[Play](https://brettdaniels2017.github.io/breakfast-fps/play.html)**

A breakfast-themed first-person shooter in one HTML page. Pack **three** weapons, pick a mode, and keep leftovers off the lot.

## Play

Promo (public): **[https://brettdaniels2017.github.io/breakfast-fps/](https://brettdaniels2017.github.io/breakfast-fps/)**  
Play (public): **[https://brettdaniels2017.github.io/breakfast-fps/play.html](https://brettdaniels2017.github.io/breakfast-fps/play.html)**

Click the game view if the browser asks for pointer lock. Pack exactly **3 of 7** guns, then start.

## What it is

Agent Scramble is a wave shooter set in diner country. You fight Hangry Eggs, Rogue Sausages, Cereal Haunts, Watermelon Brutes, Waffle Stacks, and Coffee Creeps. They melee only, path around furniture, and climb stairs.

Two modes:

- **Lot Raid** — hunt leftovers across the diner block, kitchen deck, and Salsa Cantina. Stomach HP is yours. Next wave starts 10 seconds after the last leftover dies.
- **Tower Kitchen** — hold a diner hallway. The kitchen has **1000 HP**. Leftovers chew it when they reach the counter. Hit **ORDER UP** to start each wave. Buy **Toaster Turrets** (500, then 1500 score) and **Landmines** (200 score, **G** to plant) in the Upgrades room behind the bar.

## Controls

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Look |
| Space | Jump |
| Click | Fire |
| 1–3 / scroll | Swap the three guns in your Loadout |
| Shift | Aim (Marksman 2× scope, Link Launcher 1.5× irons) |
| R | Reload |
| E | ORDER UP / buy from the shop (Tower Kitchen) |
| G | Plant a landmine (Tower Kitchen) |
| Esc | Pause (unlocks the mouse) |

## Armory

Take three of these into a run.

| Weapon | Role |
| --- | --- |
| Toast Launcher | Mid-range slices |
| Bacon Lash | Short grease whip |
| Syrup Shotgun | Close sticky blast |
| Espresso SMG | Fast spray |
| Pancake Frisbee | Thrown stack, heavy hit |
| Maple Marksman | Bolt-action sniper. Shift for a 2× scope. One shot, then a 2s bolt. |
| Link Launcher | Sausage rockets with splash. Shift for 1.5× iron sights. 3s reload. |

## Waves

Lot Raid wave 1 starts with 8 leftovers. Each later wave in a 5-round cycle is **+50%** of the last pack. Every 5th wave they get a **20% health buff** (it stacks). After a buff, pack size resets to 8. Tower Kitchen uses the same cycle at **half** the leftover count.

## Run it locally

The page loads Three.js from a CDN, so you need a local server.

```bash
cd breakfast-fps
python3 -m http.server 8766
```

Then open [http://127.0.0.1:8766/](http://127.0.0.1:8766/) for the promo, or [http://127.0.0.1:8766/play.html](http://127.0.0.1:8766/play.html) for the game.

## Project

The promo lives in `index.html`. The game lives in `play.html`. Three.js r160 loads from unpkg via an import map.

Repo: [brettdaniels2017/breakfast-fps](https://github.com/brettdaniels2017/breakfast-fps)

## Goals

- **Modes** — timed rushes, a high-score endless scramble, and a Loadout-test range.
- **Maps** — more lots besides the diner/cantina block and the Tower Kitchen hallway.
