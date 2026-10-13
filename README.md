# U10 Ringette Practice Planner

An offline practice-plan builder for U10 (FUN3 / Learn to Train) ringette. Everything is in **one file, `index.html`**: no install, no internet, no accounts.

## Getting it on your devices
- **Laptop:** double-click `index.html` to open it in Chrome, Edge, Firefox or Safari.
- **Phone or tablet at the rink:** copy `index.html` to the device (AirDrop, email it to yourself, or put it in Files/Drive set to "available offline") and open it in the browser. After that it works with no signal.
- Each browser on each device keeps **its own** saved data. Use **Guide & Data → Export JSON** to back up or move plans between devices.

## Using it
1. **Plan tab**: set the date, start time, **ice slot (50 or 60 min)**, **theme** and **ice share** (full, half or a third), then press **⚡ Auto-build plan**. It builds warm-up → 2–3 skill blocks → water → small-area game → cool-down. It only uses drills that fit your share of the ice, and it aims to keep time standing in lines under 20%.
2. **Edit the plan**: drag the ⠿ handle (touch or mouse), or use ↑ ↓ to reorder. Use − / + to change minutes, ⇄ to swap a drill (pick one yourself or press 🎲 Random swap), ✕ to remove, and add a note for each block. The summary shows total vs. slot, the estimated time in lines, how much of the practice is games, minutes per skill area, and warnings (over time, no warm-up, a drill that needs more ice than you have, and so on).
3. **🖨 Practice sheet**: one US Letter page per practice, with a rink diagram, setup, coaching cues and progressions for each drill. Press **Print / Save as PDF**. Use Letter paper, scale 100%, margins "None" or "Default".
4. **🗒 Bench card**: a compact checklist with times and the top 2 cues per drill, two copies per page (cut down the middle, one for each coach).
5. **💾 Save** stores the plan. The **Saved** tab can reopen, print or delete plans, or print them all (one page each).
6. **✔ Log as run** after practice records it in **Season** history (date, how it went, number of players, notes). The Season tab shows minutes per skill area, average time in lines and game time, and which drills you use most. **Reuse plan** copies an old practice into a new plan. Drills used in your last 3 logged practices are less likely to be auto-picked, so practices stay varied.
7. **Drills tab**: search and filter the library by category and ice area, ★ favourite drills (the auto-builder prefers favourites), and open a drill for its full card and a large diagram.

## Drill library (76 drills)
| Category | Drills |
|---|---|
| Warm-up | 9 |
| Skating & edges | 11 |
| Passing & receiving | 10 |
| Ring carrying | 8 |
| Shooting | 8 |
| Free pass & blue lines (rules) | 8 |
| Small-area games | 12 |
| Goalie basics | 5 |
| Cool-down | 5 |

Each drill has: name, skill focus, suggested duration, players/grouping, ice area (full/half/third), setup, 2–4 coaching cues, progressions and regressions, an estimated share of time spent in line, and a rink diagram drawn as SVG in code.

**Diagram key:** blue ● X = team A, red ● O = team B, ■ G = goalie, ● C = coach, orange ○ = ring, ▲ = cone, ▭ = mini-net or target. Lines: solid = skate, wavy = carry the ring, dashed = pass, thick red = shot, dash-dot = skate backward.

## Coaching principles built in
- Fun, lots of touches, small groups, one ring per player where possible.
- Under ~20% of practice time standing in lines (each drill has an estimate, and the auto-builder checks the total).
- 25–35% of the practice in small-area games.
- Short instructions with 2–3 cues, both sides and both directions, everyone gets a turn in goal.
- Ringette rules taught through drills: passing over the blue lines, 5-second free passes, crease is for the goalie only, three skaters per team in an end zone.

> Rules and U10 game formats vary by season and association. Check the current Ringette Canada rulebook and Ringette Ontario / your local association's U10 guidelines.

## Data & privacy
- Data is stored in the browser's `localStorage` under the key `ringettePlanner.v1`. Nothing is ever sent anywhere: the page has a Content-Security-Policy that blocks all network requests.
- **Export JSON** downloads a backup file and also shows the JSON in a text box you can copy (handy on iPhone). **Import** merges by default; tick "Replace instead of merge" to overwrite.
- If the browser blocks storage (e.g. some private modes), the app still works, but export before closing.

## Customising
The drills are a plain JavaScript array (`DRILLS`) near the top of the `<script>` in `index.html`. Diagrams use a small text format, documented in the comment above the array. For example: `v half; X 150,30; p 150,30 170,40; h 170,40 186,42` means half-ice view, a player, a pass, then a shot. The rink is 200 × 85 units and the right-hand net is at x = 189.
