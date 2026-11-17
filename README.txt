ZONE PDA - custom marker map for S.T.A.L.K.E.R. 2
=================================================

OPEN IT:  double-click index.html (Chrome / Edge / Firefox). No install, no server.

PLACE A PIN:  pick an icon in the sidebar (General / Factions / Anomalies),
              then click the map. Type a label, press Enter.
              Shift+click = keep placing the same icon.  Esc = cancel.
EDIT:         click a pin -> change label, notes, icon, or Delete.
MOVE:         drag the pin.
SIZE:         pins are smaller when zoomed out and grow as you zoom in.
FIND:         search box + filters; click a list entry to fly to it.
              Search also lists matches of hidden types (dimmed); clicking
              one shows that type again.

FILTERS (under the search box):
  Category checkbox      - show/hide the whole category (General, Factions,
                           Anomalies). Half-filled = some types hidden.
  Click a category name  - expand it to see one chip per type, with counts.
  Click a chip           - show/hide just that type (e.g. Thermal / Fire).
  Alt+click / right-click / "only" on a chip
                         - show ONLY that type (e.g. only Safe zone pins).
                           Do it again to show everything.
  Alt+click / right-click a category name - show only that category.
  Show all               - resets every filter.
  Placing a pin of a hidden type shows that type again automatically.

SAVING:  markers save automatically in your browser's local storage.
         That storage is per-browser (and per-computer), so to move your pins:
         Export -> copy the .json file along with this folder -> Import on the
         other machine. Export now and then as a backup too.

MAP LAYERS (top-right switch, your choice is remembered):
  Detailed map (64k)        - sharpest, but some late-game areas (Iron Forest,
                              the big northern complex) are blurry fogged
                              placeholders in the game's own texture.
  Complete map (16k)        - newer map texture, every area drawn, less sharp.
  Both line up exactly, so your pins stay put when you switch.

COURSE PLOTTER / RULER (Tools section of the sidebar):
  Plot course            - then click the map and/or pins to lay out your
                           course point by point. A dashed ruler follows the
                           cursor showing distance + time to it (and the total).
                           Clicking a pin adds it as a point (it follows the
                           pin if you move it). Click point 1 again = loop.
                           Backspace = undo last point.
                           Right-click / Esc / Enter / "Done" = stop plotting.
  On the map             - each leg shows its distance and time.
                           Click a numbered point (also the small badge next
                           to a pin) for its menu: Mark reached / x Remove.
                           Removing a pin's waypoint keeps the pin.
                           Right-click a point = remove it straight away.
                           Drag a numbered point to move it; drop it on a pin
                           (the pin glows) and it becomes that pin's waypoint.
                           Drag a pin's waypoint badge to pull the waypoint
                           off the pin (the pin itself stays put).
                           Click the line to add a bend there.
  Jog/Sprint / Walk      - pace for the time estimates, in IN-GAME time.
                           Jog/Sprint: ~20 in-game min per 500 m (measured).
                           Walk: ~40 min per 500 m (rough guess).
                           The total also lists the other pace.
  Checklist              - tick a point's box in the list (or use "Mark
                           reached" in its map menu) when you reach it. Walked legs
                           turn grey, the next point is highlighted, and the
                           panel shows "N/M reached", distance + time left and
                           the next stop (click it to fly there). Reset unticks
                           everything. Ticks are saved with the expedition.
  Point list             - click a name to fly to it, up/down to reorder,
                           x to remove.
  Undo / Fit / Clear     - drop last point / zoom to the course / remove it.
  The course is saved with your other settings.

EXPEDITIONS (saved, named courses - under the Course panel):
  Save                   - name the current course; it becomes an expedition.
                           The open expedition's name shows above the course,
                           and every change to it saves automatically.
  Save copy              - (when an expedition is open) saves it under a new name.
  New                    - start an empty course (asks before throwing away
                           an unsaved one).
  Expedition list        - newest first, each with its number of PoIs (points
                           on your pins), total points, length, time at the
                           chosen pace and creation date.
                           Click a name to open it, pencil = rename, x = delete.
  Clear                  - closes the open expedition (it stays saved).
  Deleting a pin keeps expedition points where the pin was.
  Export/Import include expeditions; importing a backup again updates the
  same expeditions instead of duplicating them.
  The list also shows checklist progress ("3/7 reached" / "done").
  Distances are approximate (~15.8 m per map unit).

COME BACK HERE (flag a pin):
  Click a pin -> "Come back here". The pin pulses with an amber ring and its
  label gets a "!" - handy for "left items here, must return".
  The ⚑ N button (top of the filters) shows only flagged pins; click again
  to show everything. Flagged pins are listed first.

PORTABLE:  copy this whole folder anywhere (USB stick, other PC).
           Both maps (zoom 0-5) are bundled in /tiles and /tiles-dlc, so it
           works offline. The detailed map's deepest zoom streams from the
           web when you're online.

Map tiles: https://github.com/joric/stalker2_tileset (thanks, joric)
