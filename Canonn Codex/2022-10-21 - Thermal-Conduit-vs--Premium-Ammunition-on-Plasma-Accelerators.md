## Thermal Conduit vs. Premium Ammunition on Plasma Accelerators

Published: 21 Oct 2022 on Canonn (https://canonn.science/codex/thermal-conduit-vs-premium-ammunition-on-plasma-accelerators/)

Content: ## Abstract

Among combat pilots there was no consensus regarding the experimental effect [Thermal Conduit](https://elite-dangerous.fandom.com/wiki/Thermal_Conduit) (TC) bonus damage for [Plasma Accelerators](https://elite-dangerous.fandom.com/wiki/Plasma_Accelerator) (PA): some were told its bonus is based on default (unengineered) weapon stats. At the same time: the same thought was regarding premium ammunition bonus damage. Both questions above lead us to the last one: do thermal conduit and premium ammunition bonus damage override/overlap each other? This study is presented by Commander Alswulf.

Video of the study by Commander Alswulf

## Setup

Since most of fights happens with ~similar configs (3 PAs or 5 PAs) – the following was used for the tests. Note that SRB stands for Short Range Blaster and means the application of the [Short Range](https://elite-dangerous.fandom.com/wiki/Short_Range_Weapon) engineering mod to the Plasma Accelerator in this case. All PAs had the TC experimental effect applied:

- Loadout 1: 3 [Efficient](https://elite-dangerous.fandom.com/wiki/Efficient_Weapon) PAs (2 Medium + 1 Huge)
- Loadout 2: 5 Efficient PAs (4 Medium + 1 Huge)
- Loadout 3: 2 Efficient PAs (Medium) + 1 SRB (Huge)
- Loadout 4: 4 Efficient PAs (Medium) + 1 SRB (Huge)

Each test was ran four times to make the following comparisons

- Cold
    - Temperature after shot should not be higher than 89% to not trigger TC bonus damage)
- Hot (Triggered TC)
    - Temperature before the shot should be higher than 150% to have its max bonus damage)
- Cold + premium ammunition
    - Premium ammunition provides +30% damage
- Hot (Triggered TC) + premium ammunition
    - Premium ammunition provides +30% damage

The following target was used for these tests

- Stock  Fer-de-Lance (FDL)
- 5C shield generator with no engineering resulting in 410 MJ of shields (or 1025 J with 4 pips into SYS for convenient calculations)

## Testing

Keeping in mind the Plasma Accelerator’s damage partition is 60% of absolute damage, 20% of thermal damage, and 20% of kinetic damage onto shields (no engineering) with 40% kinetic damage resistance and -20% thermal damage resistance.

| Test # | Loadout | Cold/Hot | Premium Ammo | Shield Damage | TC Triggered<br>Bonus Damage |
| --- | --- | --- | --- | --- | --- |
| 1 | 1 | Cold | No | 287 | — |
| 2 | 1 | Hot | No | 451 | 164 (60%) |
| 3 | 2 | Cold | No | 410 | — |
| 4 | 2 | Hot | No | 656 | 246 (60%) |
| 5 | 3 | Cold | No | 349 | — |
| 6 | 3 | Hot | No | 554 | 205 (60%) |
| 7 | 4 | Cold | No | 482 | — |
| 8 | 4 | Hot | No | 759 | 277 (60%) |

As shown in the results above, for a given loadout, triggering TC results in a 60% increase in shield damage. As such, TC bonus damage is based on the actual weapon damage (including engineering). As such, higher damage results in more bonus damage (numerically). 

| Test # | Loadout | Cold/Hot | Premium Ammo | Shield Damage | Premium Ammo<br>Bonus Damage |
| --- | --- | --- | --- | --- | --- |
| 9 | 1 | Cold | Yes | 349 | 62 (22%) |
| 10 | 1 | Hot | Yes | 554 | 103 (23%) |
| 11 | 2 | Cold | Yes | 513 | 103 (25%) |
| 12 | 2 | Hot | Yes | 820 | 164 (25%) |
| 13 | 3 | Cold | Yes | 410 | 61 (18%) |
| 14 | 3 | Hot | Yes | 656 | 102 (18%) |
| 15 | 4 | Cold | Yes | 574 | 92 (19%) |
| 16 | 4 | Hot | Yes | 912 | 153 (20%) |

As shown in the results above, the bonus damage for premium ammo is not the 30% stated by the synthesis but it is unaffected by TC being triggered or not (within rounding error).

## Conclusions

For Thermal Conduit: The numerical bonus damage is based on the damage of the weapon including engineering (a SRB PA will have a numerically higher TC damage bonus then an Efficient PA). The percentage increase is constant Additionally the bonus damage does not override the premium ammunition bonus, it is calculated independently.

For Premium Ammunition: It seems that the bonus damage for premium ammunition is based on the “default” weapon damage. Note Test #9 and Test #13, there is no difference in premium ammo damage between SRB PAs. The bonus damage should be higher and a study into the damage tests for premium ammunition for different types of engineering may be in order. It is also noted the bonus damage does not override the TC bonus, it is calculated independently and adds after TC but based on the non-engineered weapon stats.