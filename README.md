# ☢ Zone PDA — a blind field map for S.T.A.L.K.E.R. 2

A PDA-styled map of the Zone that starts **empty**. You fill it in yourself as you explore: stashes, anomalies, safe houses, faction camps, and "I left my loot here, come back later" spots.

**Live:** https://aravill.github.io/stalker-2-pda/ (or just open `index.html` locally — no install, no server)

---

## What this is (and what it isn't)

> **This is a blind map.** It doesn't know where anything is, and that's the point.

Sites like [Map Genie's STALKER 2 map](https://mapgenie.io/stalker-2) show you every stash, artifact and secret up front. That's great for 100%-ing the game, but it spoils exploring. Zone PDA works the other way round: you get the bare map texture and a set of markers, and **you record what you find, the way a stalker's PDA would**. Nothing is pre-filled or spoiled.

## 🤖 Fully vibe coded

Every line of this project was written by an AI (Claude) from plain-language requests. No hand-written code. It works, it's been tested, but treat it as a fun side project rather than carefully engineered software.

---

## Features

- **Custom pins** with labels and notes, from three icon sets:
  - General: danger, radiation, loot, stash, safe zone, quest…
  - Factions: Duty, Freedom, Loners, Ward, Spark, Monolith…
  - Anomalies: chemical / thermal (fire) / gravitational / electro…
- **Filters** per category and per type. For example, show *only* fire anomalies or *only* safe houses.
- **"Come back here" flag.** Flagged pins pulse on the map, and one button filters to just them.
- **Course plotter / ruler.** Click points on the map or on your pins to plot a course. You get a live ruler, the distance per leg, and estimated **in-game** travel time. Jog/Sprint is calibrated at ~20 in-game minutes per 500 m.
- **Expeditions.** Save courses under a name, with an overview of PoIs, length, time and creation date. Tick points off as you reach them, and see the remaining distance and time plus the next stop.
- **Two map layers:**
  - Detailed 64k map: sharpest.
  - Complete 16k map: newer, every area drawn. Use it for the Iron Forest and the northern complex, which are fogged placeholders on the 64k texture.
- **PDA look:** screen effects, scanlines and a status bar. Toggle the effects with **FX**.
- **Offline & portable.** Zoom levels 0–5 of both maps are bundled. The 64k map's deepest zoom levels stream from the web when you're online.

## Your data

Everything is stored in your browser's `localStorage`, on this device and in this browser only. Nothing is sent anywhere.

- **Export** downloads a `.json` backup with all pins and expeditions. **Import** loads one, and lets you merge or replace.
- The hosted version and a local copy are separate. Use Export/Import to move pins between them.

## Quick controls

| Action | How |
|---|---|
| Place a pin | Pick an icon in the sidebar, then click the map. Shift-click to keep placing. |
| Edit / delete a pin | Click the pin |
| Move a pin | Drag it |
| Show only one type | Alt-click or right-click a filter chip, or click its "only" |
| Plot a course | **Plot course**, then click the map or pins. Backspace = undo. Esc, Enter or right-click = done. |
| Edit a course | Drag points, right-click a point to remove it, click the line to add a bend |
| Mark a point reached | Tick it in the list, or click the point on the map |

More detail is in [`README.txt`](README.txt), which is the offline manual shipped with the app.

## Run it locally

```bash
git clone https://github.com/Aravill/stalker-2-pda.git
```

Then double-click `index.html`. It works in Chrome, Edge and Firefox, straight from `file://`.

## Credits

- Map tiles: [joric/stalker2_tileset](https://github.com/joric/stalker2_tileset). Thanks, joric.
- Map engine: [Leaflet](https://leafletjs.com/) 1.9.4 (bundled in `lib/`).
- S.T.A.L.K.E.R. 2: Heart of Chornobyl © GSC Game World. This is an unofficial fan tool, not affiliated with or endorsed by GSC.
