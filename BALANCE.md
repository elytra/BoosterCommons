* **No ore tripling, quadrupling, quintupling, etc. Ever.**
	* The absolute limit on ore multiplication is 2.6 ingots per ore block, with typical gains being closer to 1.6.
* **A single block can never store more than 36 disparate stacks of items, even when it's part of a multiblock structure.**
	* Barrels or other single-type storages can hold up to 64 stacks of the same item.
	* This limit should be from the end-user's point of view; a single block component of a multiblock can hold more than 36 stacks from code side, but it has to *seem* like it doesn't hold more from the player side because they need to add more blocks to the multiblock to access that extra storage.
* **A single block can never store more than 64 buckets of fluid, even when it's a part of a multiblock structure.**
	* This applies only to tanks that exist exclusively as tanks. A machine tank can never store more than 4 buckets of fluid, even when it's part of a multiblock structure.
	* This follows the end-user rule as item storage limits do.
* **Furnace-burning fuels should produce no more than 30RF per furnace fuel tick.**
	* It can produce this as slowly or as quickly as you want.
* **Wireless interactions are permissible, and a trivial wireless implementation generally performs well.**
	* However, well-designed network-topography-aware systems (i.e. wires) often outstrip the performance of wireless systems, and occasionally even dumb cellular systems do. More importantly, wireless is unsatisfying gameplay.
* **Time is _not_ a balancing mechanic.**
	* Free energy that takes a long time to generate is still free energy (this is why there are no time constraints placed on energy generation).
* **Material cost is not a balancing mechanic.**
	* An overpowered machine that requires 26 expensive casing blocks is overpowered, and also not a real multiblock machine.
* **RF is RF. Forge Energy is RF. Tesla is RF.**
	* More generally, if something is RF-compatible, the same guidelines apply.
	* This does NOT mean API or ABI compatibility. This means user-facing compatibility. If I can run power from a Salty Snacks machine to an RF machine, Salty Snacks is RF-compatible.
* **Augments > in-place upgrades > machine tiers.**
	* Direct competition between blocks from the same mod feels like material is wasted and just isn't fun.
	* An item-based, removable augment system is the best option, but in-place upgrades are acceptable as well.

## Extra Reading

* Vazkii has [some really good writing](http://vazkii.us/uncategorized/sins-of-a-solar-empire-or-the-passive-generation-conundrum/) on passive generation and why you want to avoid it.
* Vazkii *also* has [some good writing](https://www.reddit.com/r/feedthebeast/comments/5zzjek/fake_players_a_discussion_about_limiting_options/df2obsy/) on target audience, and why configurability can be bad.
* Extra Credits has a [whole video](https://www.youtube.com/watch?v=EitZRLt2G3w) on first-order optimization.
  * This is really important, and it seems like we aren't getting it as modpack creators. Please think about these things. They matter.
