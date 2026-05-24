# Defenses

## Evasion Rating

Evasion Rating (EV) itself has no hard cap - you can stack as much as your gear,
passives, and buffs allow. What's capped is the resulting chance to evade: it is
soft-capped at 95 %, so you can never be un-hittable. The conversion from rating
to evade chance follows a diminishing returns formula based on the attacker's
accuracy and level.

- **Diminishing returns set in fast.** Doubling your EV does not double your
  evade chance - each additional point contributes less. There's a sweet spot
  per character level beyond which extra rating yields very little.
- **Evasion is entropy-based, not a fresh dice roll per hit.** PoE 2 tracks
  accumulated evade chance, so long streaks of taking consecutive hits are far
  less likely than pure RNG would suggest. 95 % evade ~ roughly 1 in 20 hits
  land, distributed evenly.
- **Evasion does nothing against spells or damage-over-time.** Spells need spell
  suppression or block, DoTs (poison, ignite, burning ground, bleed) ignore EV
  entirely.
- **Monster accuracy scales with area level.** Pure EV gets weaker in maps
  unless you also stack life, armour, or ES - high-level Rares and Bosses have
  enough accuracy to chunk through even 95 % EV on an unlucky entropy roll.

### Evasion Rating Sweet Spot by Character Level

The in-game character sheet shows your estimated evade chance against a **normal
monster of your character level**. Use the table below to gauge how much EV is
worthwhile at each stage of the game.

Formula used: `Chance to Hit = 1.25 × A / (A + (EV ÷ 5)^0.9)`, where A is
monster accuracy. Monster accuracy approximated as `5.92 × level + 40`.
Verified at level 84 (A ≈ 538): 20 000 EV → ~70.5 % evade.

| Char Level | ~Monster Acc. | 60 % evade | **75 % evade ★** | 85 % evade |
|:----------:|:-------------:|:----------:|:----------------:|:----------:|
| 1 – 15     | ~100          | ~2 000     | **~3 900**       | ~7 600     |
| 16 – 30    | ~190          | ~3 900     | **~7 900**       | ~15 400    |
| 31 – 45    | ~277          | ~6 000     | **~12 100**      | ~23 700    |
| 46 – 55    | ~336          | ~7 400     | **~15 000**      | ~29 400    |
| 56 – 65    | ~396          | ~8 900     | **~18 000**      | ~35 200    |
| 66 – 74    | ~455          | ~10 400    | **~20 900**      | ~41 000    |
| 75 – 82    | ~514          | ~11 900    | **~24 000**      | ~47 100    |
| 83+ (T16)  | ~538          | ~12 500    | **~25 300**      | ~49 500    |

**★ 75 % is the practical sweet spot.** Going from 60 % → 75 % costs roughly
double the EV but halves the hits you take. Pushing above 85 % costs 2–3× more
EV again for a marginal gain; 90 % evade requires ~82 000 EV at level 84 and is
only realistic on dedicated late-game builds.

> **Caveats:** These values are against *normal* monsters. Rare monsters and
> bosses have higher accuracy, so your effective evade chance will be lower than
> your character sheet shows against them. Map mods such as "monsters have
> increased Accuracy Rating" further raise the bar.

---

## Sources

- [Evasion - Path of Exile 2 Wiki (poewiki.net)](https://www.poewiki.net/wiki/poe2wiki:Evasion)
- [Accuracy - Path of Exile 2 Wiki (poewiki.net)](https://www.poewiki.net/wiki/poe2wiki:Accuracy)
- [PoE 2 Guide: Evasion Explained (Mobalytics)](https://mobalytics.gg/poe-2/guides/evasion)
- [PoE 2 Guide: Accuracy Explained (Mobalytics)](https://mobalytics.gg/poe-2/guides/accuracy)
- [PoE 2 Evasion Mechanics Guide (ggwtb.com)](https://ggwtb.com/blog/poe-2-evasion-mechanics-guide-how-to-works)
- [How Evasion Changes Affect Build Defense Mechanics (poecurrency.com)](https://www.poecurrency.com/news/poe-2-how-evasion-changes-affect-build-defense-mechanics)
- [Path of Exile Mechanics Explained: Evasion & Entropy System (poecurrency.com)](https://www.poecurrency.com/news/path-of-exile-evasion-entropy-system)
- [How Evasion Works in PoE 2 - Forum Thread (pathofexile.com)](https://www.pathofexile.com/forum/view-thread/3648860)
