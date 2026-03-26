# FireDash

A retro-styled 2D endless runner web game — inspired by the Chrome Dino, but you're a **fireman** dodging hilariously random obstacles.

## Play

Open `index.html` in any modern browser. No build step, no dependencies — just one file.

## Controls

| Platform    | Jump              | Duck                |
| ----------- | ----------------- | ------------------- |
| **Desktop** | `Space` / `Click` | `Arrow Down` (hold) |
| **Mobile**  | JUMP button       | DUCK button (hold)  |

On desktop, on-screen buttons can be enabled via the settings gear in the top-left corner.
On mobile, on-screen buttons are always visible.

## Gameplay

- The fireman runs automatically. Jump over **ground obstacles** and duck under **air obstacles**.
- **10 ground obstacles**: Fire Hydrant, Cat, Donut, Banana Peel, Rubber Duck, Traffic Cone, Trashcan, Cactus, Tire, Mailbox
- **5 air obstacles** (appear after 80 pts): Bird, Plane, Bat, UFO, Drone — duck to survive.
- Speed increases **every 200 points**.
- At **1000 points** the colors flash and the game switches to **dark mode** (night). Every 1000 points it toggles back and forth.

## Background Scenes

Scrolling background features random firefighter scenarios:

- **Ladder rescue** — a cat stuck on a building
- **Flood response** — sandbags and a rescue boat
- **Car crash** — two vehicles with a firefighter on scene
- **Tower fire** — buildings with smoke and a water hose stream

## Scoring

- Points accumulate from distance and passing obstacles (+10 each).
- **Session highscore** saved via `sessionStorage` (persists until the tab is closed).
- Beat your record to see a "New Personal Best!" message.

## Mobile Support

- Fully responsive with larger scaling for touch devices.
- Dedicated JUMP / DUCK buttons.
- Zoom and scroll prevention for smooth gameplay.

## Audio

All sound effects are generated via Web Audio API (no external files):

- Jump, Duck, Game Over, and Mode Change sounds.

## Tech

- **Single file**: HTML + CSS + JS in one `index.html`.
- **Canvas 2D** rendering with DPR-aware scaling.
- Zero dependencies.
