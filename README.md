# The Stolen Lands & the Kingdom Thereof

An interactive chronicle of a Kingmaker Adventure Path campaign, run under
Starfinder 2e rules by our GM for the Dayton table. Live at
**https://kingmaker.endlessrpg.com**.

The map tracks the party's exploration of the Stolen Lands hex by hex —
fog of war, surveyed and claimed territory, provinces, settlements, points
of interest, and a session chronicle — with the whole table able to
contribute under role-based permissions.

## How it works

- **Hosting:** a single static HTML file served by GitHub Pages. No build step.
- **Kingdom data:** [Supabase](https://supabase.com) (Postgres + Google login).
  Row-level security enforces three roles: **GM** (full control, including
  revealing territory), **Editor** (may develop hexes the GM has revealed),
  and **Visitor** (read-only). All changes sync live to every open copy.
- **Kingdom mechanics:** read live from the group's Royal Kingdom Sheet
  (Google Sheets). The spreadsheet remains the single source of truth for
  settlements, structures, and kingdom-turn math; the map displays it.
- **The grid:** 29×12 hexes (columns A–AE, skipping I and O; 346 playable
  cells under the ≥50%-visible rule), calibrated to the map artwork to
  sub-pixel accuracy.

`campaign.json` in this repo is a periodic snapshot of the kingdom's state,
kept as a backup and historical record; the database is authoritative.

## Acknowledgements

- **Map of the Stolen Lands** by **Dimitris Havlidis**
  ([worldanvil.com](https://www.worldanvil.com)), shared freely with the
  community. The map image remains his work and is not covered by this
  repository's license.
- **Royal Kingdom Sheet** by **Tom-Eric Gerritsen**, with Moreno Corputtij
  and community contributors, under the Open Game License v1.0a.
- **Kingmaker** is a Paizo Inc. adventure path. This is an unofficial,
  non-commercial fan project for a single home campaign, made under Paizo's
  Community Use Policy. We claim no ownership of Paizo's material.
- Adapted to Starfinder 2e and run, with patience, by **Brent** — and played
  by the Dayton table, whose hot-pink post-it notes this site replaces.

Built by Chad & Claude, 2026.
