# Changelog

Rough version history for the Collectable Leveling Ledger, grouped from the
commit log. `X.Y.Z`: `Y` bumps for a notable new feature, `Z` bumps for
smaller fixes/tweaks within that feature set. `X` is reserved for a full
rewrite and hasn't moved yet.

## 1.9.1 -- 2026-09-20
- Fix raw material counts not shrinking when a component is set to "buy"
  instead of crafted (e.g. unchecking 18 Acacia Lumber now also drops the
  90 Acacia Logs that would've gone into crafting them)

## 1.9.0 -- 2026-09-20
- Add in-game item icons to each job's turn-in breakdown
- Show each collectable's level next to its name

## 1.8.2 -- 2026-09-20
- Rearrange job card inputs: current/target level side by side, Current EXP
  in a bigger box below, matched in height and font size to the others

## 1.8.1 -- 2026-09-20
- Cap the Current EXP input to the level's own digit count, blocking
  over-cap typing outright instead of clamping after the fact

## 1.8.0 -- 2026-09-20
- Add TeamCraft import links split by recipe-unlock bracket (per job and
  consolidated), via a modal with separate "buying every component" and
  "crafting your own" sections
- Correct the recipe-unlock brackets to 71-75/75-80/80-85/85-90/90-95/95-100
  and cap the Cosmic Exploration / Ishgardian Restoration mentions at 71
- Rewrite the hint paragraph's crafting-window explanation

## 1.7.2 -- 2026-09-20
- Hide "gather my own raw materials" until crafting is fully on
- Restore the max-collectability caveat; fix custom-target detection
- Prompt to re-fetch prices when the summary has unpriced items

## 1.7.1 -- 2026-09-19
- Fix "Buying components" silently using craft cost for craft-toggled items
- Respect "gather my own raw materials" for top-level raw ingredients too
- Assorted layout fixes: breakdown cards overflowing their border, opened
  breakdowns not scrolling into view, unrelated re-renders jumping the page

## 1.7.0 -- 2026-09-19
- Rework the buy/craft/gather toggles: a real per-component Craft checkbox,
  a Gather checkbox added to the components table too, every component
  defaults to Craft when the job crafts its own
- Add a consolidated price breakdown across all jobs combined

## 1.6.2 -- 2026-09-19
- Price items by average recent sale instead of the single cheapest listing
- Move the gil summary next to the EXP summary
- Block turning off "craft my own components" while gathering is on
- Persist item names locally so reloads don't lose them; various dropdown fixes

## 1.6.1 -- 2026-09-19
- Only fetch gil prices on demand, cache them for 10 minutes, and surface
  Universalis rate limits

## 1.6.0 -- 2026-09-19
- Add a "gather my own raw materials" toggle with per-item override
  checkboxes; render the gil breakdown as a proper table

## 1.5.0 -- 2026-09-19
- Add a gil cost estimate via Universalis market prices: collapsible
  per-job price breakdown, cascading data center/world dropdowns, items
  linked to their Universalis listing

## 1.4.1 -- 2026-09-19
- Fix misleading hint text around component crafting; drop the
  "experimental" label now that the gating is correct

## 1.4.0 -- 2026-09-19
- Add self-crafted-component EXP calculation: simulate all 8 jobs jointly
  so cross-job EXP credit actually applies, gate component crafting by
  Dawntrail's real batched recipe unlocks, per-component and
  select-all/deselect-all toggles
- Split the EXP breakdown into "crafting" vs "crafting (components)"

## 1.3.1 -- 2026-09-19
- Link to TeamCraft's Lists page next to the consolidated import button

## 1.3.0 -- 2026-09-19
- Add job icons for each Disciple of the Hand (official XIVAPI class icons)

## 1.2.1 -- 2026-09-19
- Assorted code-review fixes; trim job-note wording

## 1.2.0 -- 2026-09-19
- Extend collectable data down to level 71 (previously started higher) and
  default all jobs to level 71

## 1.1.1 -- 2026-09-19
- Persist job inputs across reloads (localStorage)
- Fix input misalignment when the "Target lv" label wraps; fix a dead
  "already level 100" message

## 1.1.0 -- 2026-09-19
- Replace the flat craft-completion EXP bonus with the game's real formula
- Add a per-job and overall EXP source breakdown (turn-ins vs. crafting)
- Add a consolidated TeamCraft import link across all jobs

## 1.0.0 -- 2026-09-19
- Initial release: leveling calculator for all 8 crafting jobs via
  Rarefied collectable turn-ins
