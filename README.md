# Ringette Practice Planner (U10 + Learn to Skate)

An offline practice-plan builder with two levels, picked with the **U10 / Learn to Skate** switch at the top of the page:
- **U10** (FUN3 / Learn to Train): the original planner, unchanged.
- **Learn to Skate**: roughly U7/U8 Active Start, first-time skaters and weak skaters.

Everything is in **one file, `index.html`**: no install, no internet, no accounts.

## Getting it on your devices
- **Laptop:** double-click `index.html` to open it in Chrome, Edge, Firefox or Safari.
- **Phone or tablet at the rink:** copy `index.html` to the device (AirDrop, email it to yourself, or put it in Files/Drive set to "available offline") and open it in the browser. After that it works with no signal.
- Each browser on each device keeps **its own** saved data. Use **Guide & Data → Export JSON** to back up or move plans between devices.

## Using it
0. **Pick the level** with the switch in the header. Each level keeps its own draft plan, ice-slot options, themes, drill library and season stats, so switching back and forth doesn't lose anything. Saved plans from both levels are listed together (with a level badge), and opening one switches to its level.
1. **Plan tab**: set the date, start time, **ice slot (50 or 60 min)**, **theme** and **ice share** (full, half or a third), then press **⚡ Auto-build plan**. It builds warm-up → 2–3 skill blocks → water → small-area game → cool-down. It only uses drills that fit your share of the ice, and it aims to keep time standing in lines under 20%.
2. **Edit the plan**: drag the ⠿ handle (touch or mouse), or use ↑ ↓ to reorder. Use − / + to change minutes, ⇄ to swap a drill (pick one yourself or press 🎲 Random swap), ✕ to remove, and add a note for each block. The summary shows total vs. slot, the estimated time in lines, how much of the practice is games, minutes per skill area, and warnings (over time, no warm-up, a drill that needs more ice than you have, and so on).
3. **🖨 Practice sheet**: one US Letter page per practice, with a rink diagram, setup, coaching cues and progressions for each drill. Press **Print / Save as PDF**. Use Letter paper, scale 100%, margins "None" or "Default".
4. **🗒 Bench card**: a compact checklist with times and the top 2 cues per drill, two copies per page (cut down the middle, one for each coach).
5. **💾 Save** stores the plan. The **Saved** tab can reopen, print or delete plans, or print them all (one page each).
6. **✔ Log as run** after practice records it in **Season** history (date, how it went, number of players, notes). The Season tab shows minutes per skill area, average time in lines and game time, and which drills you use most. **Reuse plan** copies an old practice into a new plan. Drills used in your last 3 logged practices are less likely to be auto-picked, so practices stay varied.
7. **Drills tab**: search and filter the library by category and ice area, ★ favourite drills (the auto-builder prefers favourites), and open a drill for its full card and a large diagram.

## Learn to Skate level
- **Ice slot 45 or 50 min.** Templates:
  - 45 min: helmet check & warm-up 5 → skill 7 → skill 6 → water 2 → station rotation 10 → fun game 11 → cool-down huddle 4
  - 50 min: warm-up 6 → skill 7 → skill 7 → water 2 → station rotation 12 → fun game 12 → cool-down 4
- **Themes:** balanced mix, first time on ice (balance & falling), marching/gliding/striding, stopping (snowplow), backward skating, edges/turns/crossover intro, ring & stick fun.
- **Minimal lining up:** the auto-builder targets **under 15% of time in lines** (U10 target is 20%) by using everyone-at-once drills, waves of 4–5 across the width of the ice, and 3–4 short stations with a coach at each.
- **Coach-to-skater ratio:** enter *skaters expected* and *coaches/helpers on ice*. The summary shows the ratio and warns above 1:6, with a stronger warning above 1:8 (aim for 1:3–4 with first-timers). This is planning guidance; check your association's ratio and helper-screening rules.
- **Safety cues:** helmet/chin-strap check in the warm-up, safe falling and the *bear → knight → stand* get-up, plus a helmet and ratio reminder on every practice sheet and bench card.
- Warnings tell you when there's no fun game, a block runs longer than 12 minutes, there's no station rotation in a skill-heavy plan, or the ratio is too high.
- In the drill picker and the Drills tab, tick **All levels** to borrow drills from the other level (for example, Learn to Skate drills for weak skaters in a U10 practice).

### Learn to Skate library (57 drills)
| Category | Drills |
|---|---|
| Warm-up | 6 |
| Balance & falling | 6 |
| Marching, gliding & stride | 8 |
| Stopping | 4 |
| Backward skating | 4 |
| Edges, turns & crossovers | 6 |
| Ring & stick | 6 |
| Fun games | 9 |
| Short stations | 5 |
| Cool-down | 3 |

Examples: Fall Down, Get Up (Bear, Knight, Stand); Penguin March; March & Glide; Two-Foot Glide Record; Swizzles (Make Lemons); Snowplow Stop – Pizza!; Scooter Pushes; Big Pushes – Stride Basics; Backward Wiggle and Backward Swizzles; Circle Glides; Crossover Step-Overs; Ring Push March; Feed the Monster; Ring Bowling; Red Light, Green Light; Sharks and Minnows; Obstacle Course Adventure; Pirate Treasure Hunt; Tail Tag; Clean Your Room; Crocodile River; Musical Islands; Cross-Ice Ring Game; and five station circuits (including one for ⅓ ice).

## U10 drill library (76 drills)
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
- Older backups and data from the U10-only version load as U10 plans. Nothing needs converting.
- Data is stored in the browser's `localStorage` under the key `ringettePlanner.v1`. Nothing is ever sent anywhere: the page has a Content-Security-Policy that blocks all network requests.
- **Export JSON** downloads a backup file and also shows the JSON in a text box you can copy (handy on iPhone). **Import** merges by default; tick "Replace instead of merge" to overwrite.
- If the browser blocks storage (e.g. some private modes), the app still works, but export before closing.

## Customising
The drills are plain JavaScript arrays near the top of the `<script>` in `index.html`: `DRILLS` (U10) and `LTS_DRILLS` (Learn to Skate, appended to `DRILLS` with `lvl: "lts"`). Level settings (slots, themes, templates, line target, categories) are in `LEVELS`, and the ratio thresholds are in `LTS_RATIO`. Diagrams use a small text format, documented in the comment above the array. For example: `v half; X 150,30; p 150,30 170,40; h 170,40 186,42` means half-ice view, a player, a pass, then a shot. The rink is 200 × 85 units and the right-hand net is at x = 189.
