# Changelog

What's changed in the Collectable Leveling Ledger, roughly grouped into
versions.

## 1.10.0 -- 2026-09-20
- Replaced the default scrollbar with a thinner, more minimal one, including
  inside the Changelog window
- Current level and Target lv now use matching, custom-styled up/down
  buttons; Current EXP no longer shows them

## 1.9.1 -- 2026-09-20
- Fixed: unchecking a component you'd rather buy than craft now also removes
  the raw materials it would've needed from your shopping list (e.g. skip
  crafting your own lumber and the logs behind it disappear too)

## 1.9.0 -- 2026-09-20
- Added each collectable's in-game icon and level to the turn-in list

## 1.8.2 -- 2026-09-20
- Rearranged the job card layout: current/target level side by side, with a
  bigger Current EXP box below

## 1.8.1 -- 2026-09-20
- The Current EXP box no longer lets you type more digits than that level
  actually allows

## 1.8.0 -- 2026-09-20
- Added TeamCraft import links split by level range
- Corrected the level ranges used for those links to match how recipes
  actually unlock (71-75, 75-80, 80-85, 85-90, 90-95, 95-100)
- Clarified the explanation of how leveling before 71 and the crafting
  windows after it work

## 1.7.2 -- 2026-09-20
- Restored a note clarifying that turn-ins need max collectability to earn
  full EXP
- Added a prompt to re-fetch prices when some items are showing as unpriced
- Hid the "gather my own raw materials" option until crafting your own
  components is fully turned on

## 1.7.1 -- 2026-09-19
- Fixed the "buying every component" cost sometimes quietly using the
  crafting cost instead
- Fixed raw materials you'd already marked as free-gathered still getting
  charged in some cases
- Various scrolling/layout fixes to the price breakdown panels

## 1.7.0 -- 2026-09-19
- Reworked the buy/craft toggles so every individual component (not just
  whole jobs) can be switched between "buy it" and "craft it yourself"
- Added a combined price breakdown across all 8 jobs at once

## 1.6.2 -- 2026-09-19
- Prices are now based on the average of recent sales instead of just the
  cheapest listing
- Moved the gil cost summary next to the EXP summary
- Various small dropdown and layout fixes

## 1.6.1 -- 2026-09-19
- Prices are now only fetched when you ask for them, and are reused for 10
  minutes
- Added a clearer message if Universalis is temporarily unavailable

## 1.6.0 -- 2026-09-19
- Added a "gather my own raw materials" option that treats gatherable
  materials as free, with the ability to uncheck specific ones you'd rather
  buy anyway

## 1.5.0 -- 2026-09-19
- Added estimated gil costs for turn-ins, pulled from live Universalis
  market prices for your chosen data center and world
- Added a collapsible price breakdown per job showing exactly what you'd
  need to buy

## 1.4.1 -- 2026-09-19
- Clarified the explanation text around crafting your own components

## 1.4.0 -- 2026-09-19
- Added the option to craft your own components instead of buying them,
  with EXP credit shared correctly across all 8 jobs and unlock timing that
  matches Dawntrail's actual recipe-unlock schedule
- Split the EXP breakdown so crafting your final collectable and crafting
  its components are shown separately

## 1.3.1 -- 2026-09-19
- Added a link to TeamCraft's Lists page next to the import button

## 1.3.0 -- 2026-09-19
- Added an icon for each crafting job

## 1.2.0 -- 2026-09-19
- Added collectables down to level 71, covering the full 71-100 leveling range

## 1.1.1 -- 2026-09-19
- Your entered levels and EXP are now remembered when you reload the page
- Fixed a couple of small display glitches

## 1.1.0 -- 2026-09-19
- EXP from crafting now uses the game's real formula instead of an
  approximation
- Added a breakdown showing how much EXP comes from turn-ins vs. crafting
- Added a single TeamCraft import link covering every job at once

## 1.0.0 -- 2026-09-19
- Initial release: a leveling calculator for all 8 crafting jobs based on
  turning in Rarefied collectables
