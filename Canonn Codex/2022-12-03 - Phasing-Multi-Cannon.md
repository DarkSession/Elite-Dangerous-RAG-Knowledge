## Phasing Multi-Cannon

Published: 03 Dec 2022 on Canonn (https://canonn.science/codex/phasing-multi-cannon/)

Content: ## Abstract

During Disrupt Azimuth’s Resource Campaign commanders who supported it were able to get as reward a unique weapon: pre-engineered multi-cannon with phasing experimental effect.
The last part is what we would expect to be “unique” since there is no other in-game way to make phasing multi-cannons. But it was found out that phasing is not the only “uniqueuesness”. At the same time there was a question of its “effectiveness”.
Commanders who get into top 25% of that CG were able to get 2 medium pre-engineered phasing multicannons.

Video of the study by Commander Alswulf

## Setup

According to in-game stats, the pre-engineered weapon has 3 combined engineered modifications: rapid fire, short range and high capacity.
Basic stats change are:

- DPS: 59.1/s (+278%)
- Maximum Range: 2000m (-50%)
- Rate of Fire: 10/s (+40%)
- Ammo Clip Size: 400 (+300%)
- Ammo Maximum: 6400 (+204.8%)
- Rounds per Shot: 3 (+200%)
- Jitter: 3°
- Falloff: 1800m (-10%)

At first, a small test was done (Test #1): ammo clip depletion compare to non-engineered multi-cannon. It was found that time to deplete was the same.

Additional testing was done as follows:

- To check damage partition, a Guardian SLF Lance with 10 hull was used
- To check distance vs damage, a FDL with 1048 hull was used (shield strength was irrelevant due to phasing potential)
- To check the effectiveness during PVE, a wing mission to destroy NPC engineered FDLs was used with 2 Federal Assault Ships with the following configurations:
    - 2 Large gimballed rapid fire phasing pulses + 2 CG pre-engineered phasing multi-cannons
    - 2 Large fixed + gimballed incendiary + corrosive multi-cannons + 2 CG pre-engineered phasing multi-cannons

## Testing

#### Test #2

It’s known that phasing damage is 10% of weapon damage (including engineering) which pierce shields and applies to the hull as absolute damage (ignoring hull resistances) on shielded targets. This test was made at point-blank distance. Keeping in mind Elite’s rounding:

- Hull Damage to Lance per 1s
    - Expected: ~60%
    - Actual: 58%
- Time to Phase Lance Hull
    - Expected: ~1.8s
    - Actual: 1.74s

#### Test #3 – Test #10

The following tests were done to assess the effect of distance on the multi-cannon’s damage. As stated before a FDL was used as a target with the goal of removing 10% of the hull. Two attack profiles were used, one on the top and one on the front. The results are tabulated below and shown in the plot.

| Test # | Distance [m] | Ship Profile | Time to 105 (10%) Hull Damage [s] |
| --- | --- | --- | --- |
| 3 | 235 | Up Side | ~10 |
| 4 | 500 | Up Side | ~10.4 |
| 5 | 1000 | Up Side | ~14 |
| 6 | 1500 | Up Side | ~25.5 |
| 7 | ~1990 | Up Side | ~38 |
| 8 | 500 | Front Side | ~12.9 |
| 9 | 1000 | Front Side | ~26.7 |
| 10 | 1500 | Front Side | ~47.8 |

![](https://canonn.science/wp-content/uploads/2022/12/PhasingMultiPlot.png)

#### Test #11 and Test #12

| Test # | Config | Phased Hull Before Shields Dropped | Time to Destroy Engineered NPC FDL |
| --- | --- | --- | --- |
| 11 | 2 Large gimballed Rapid fire phasing pulses + 2 CG pre-engineered phasing multi-cannons | ~55% | ~5:50 |
| 12 | 2 Large fixed + gimballed incendiary + corrosive multi-cannons + 2 CG pre-engineered phasing multi-cannons | ~16% | ~3:50 |

## Conclusions

CG phasing multi-cannons look workable. Even without counting phasing as an experimental – the damage for the medium class weapon is very high. It’s phasing potential is also higher than any huge laser weapons can provide. Keeping in mind “not that good” distance control with the FAS – it’s possible to deal decent damage. Jitter denies huge damage portions depending on distance and the defending ship’s profile.
More stats are required to find more usable configurations in scope of player-vs-player (PVP) combat.