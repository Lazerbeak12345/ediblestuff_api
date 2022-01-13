# The Edible Stuff API Mod

[![ContentDB](https://content.minetest.net/packages/lazerbeak12345/ediblestuff_api/shields/downloads/)](https://content.minetest.net/packages/lazerbeak12345/ediblestuff_api/)

Adds an API to MineTest to easily register tools as edible - and to make
specified armor get "eaten" automatically when hunger goes down.

When an `edible_while_wearing` armor peice is equipped, the player will eat some
of that armor if their saturation (or health in absence of a hunger 
mod) is below 85%. This reduces the durability of a random armor piece.

This mod was created for the [`chocolatestuff`][cs] mod, and so you can make your own armors like it - without needing to depend on `farming`.

[cs]: https://github.com/Lazerbeak12345/chocolatestuff

## Requires

Nothing! But it has optional integration with:

- `stamina`
	- the `minetest-mods` fork
	- the `TenPlus1` fork
	- the `sofar` fork
- `hbhunger`
- `hunger_ng`
- `3d_armor`
	- If absent the armor apis do nothing.

## TODO

- [ ] Upstream bug in 3d_armor with `get_weared_armor_elements`
- [ ] make a way to actually use the tool (shift? no shift?)
  - Doesn't seem possible. Can't tell MT engine to eat the tool but not use tool (except hoe, which is a type defined in farming)
- [ ] delete functions after mods loaded (using event - not timer)
- [ ] Settings?

## Legal

Copyright 2021-2 Lazerbeak12345

### Credit

- The YourLand players for a bunch of questionable ideas for this questionable mod. Original idea was from "Bla."
- The creator of [the obsidianstuff redo mod](https://github.com/OgelGames/obsidianstuff). This takes inspiration from that repo.
- The creator [the edible swords mod][the_edible_swords_mod]. I took inspiration from this repo as well.

### Licence

Due to the dependancy on instant_ores, this mod _must_ be gpl 3 or later compatible. Thus, this mod is under GPL 3.0 or later.
