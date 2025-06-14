## Advanced Multi-Cannon Analysis

Published: 03 Jun 2019 on Canonn (https://canonn.science/codex/advanced-multi-cannon-analysis/)

Content: ### 1. Introduction

The galactic community recently decided to support Zende Partners in the development of an Advanced Multi-Cannon (AMC) weapon [1].  Given the usual lack of transparency in weapon documentation, the goal of this study was to characterize the Anti-Xeno (AX) properties of this newly developed module.  Additionally, after the basic AX damage properties of the weapon were measured, it was discovered that the AMCs have the unique ability to help us estimate the AX resistance of human shields and hull plating.  A “bonus” analysis was therefore carried out to estimate the AX resistance of human technology.

### 2. Executive Summary

Mathematical and experimental rigor was used to estimate the AX damage properties of the newly developed Advanced Multi-Cannon.  The following facts were uncovered in this analysis:

1. When configured with AX ammunition, 100% of the weapon’s damage output is converted to AX damage.
2. The damage per shot and Armor Piercing of the AMC are indeed 2.2 and 37, respectively.
3. Human shields have a resistance to AX damage of 95%.
4. Human armor plating has a resistance to AX damage of 90%.

The above resistance values will be used in a future study to re-estimate the damage partitioning of other human and Guardian AX weapons.

### 3. Theory

Here we employ the basic damage equation that was originally formulated in the Thargoid shield analysis [2], in which damage was tested against a Cyclops Interceptor’s shield:

![](https://canonn.science/wp-content/uploads/2019/04/XX_03_equation_1_revised.png)

where *δ* is the full weapon damage figure, *N* is the total number of weapon shots fired, *ω\_a* is the AX component of the full damage,  *ω\_n* is the “normal” or conventional component of the full damage, *ρ\_a* is the resistance of the Thargoid’s shield to AX damage, *ρ\_n* is the resistance of the Thargoid’s shield to the weapon’s conventional damage (which can be thermal, kinetic, explosive, or absolute), *S* is the Cyclop’s shield strength, and ∆ is the fraction of the shield strength at a given moment after the Interceptor has activated its shield.  In this analysis we will be making the assumption that Thargoids have no resistance (or enhancement) to AX damage, so we will set to *ρ\_a* to zero.

We know that the two fractional damage components must add up to unity:

![](https://canonn.science/wp-content/uploads/2019/04/XX_04_equation_2.png)

Additionally, the weapon damage value that is listed in the outfitting screen is just the product of the full damage and its corresponding scaling factor:

![](https://canonn.science/wp-content/uploads/2019/04/XX_05_equation_3.png)

Plugin in the two equations above into the basic damage equation, we can solve for the full weapon damage *δ*:

![](https://canonn.science/wp-content/uploads/2019/04/XX_06_equation_4.png)

Once we have the full weapon damage, we can estimate the fractional components of the AMC. The cyclops shield strength and its resistances were measured in a previous analysis [2]. The parameter ∆ and the number of shots fired are values that are measured experimentally.

### 4. Results

The data acquisition and experimental methodology used in this analysis is the same one employed in the shield strength analysis [2].  In this study we used three (unengineered) C2 Advanced Multi-Cannons in order to reduce the Cyclops shield as much as possible in a short period of time.  Each cannon was configured to deliver AX damage.  A total of three experimental trials were conducted and the results were averaged together as shown below.

![](https://canonn.science/wp-content/uploads/2019/06/ZZZZ_01_AMC_damage_partition_results_v2-1024x166.png)

We hypothesized that all of the damage delivered by the weapon is attributed to the AX component.  The results above indicate that the damage attributed to the normal, i.e. kinetic, component of the damage is essentially zero, within the experimental uncertainties.  It’s possible the full weapon damage is actually closer to 2.18, as indicated by the averaged results, but we can’t make that conclusion with certainty given the slight errors in the experiment.

The fact that *all* of the damage delivered by an AX-configured AMC is actually a surprising result, which, as will be explained in the next section, will allow us to conduct more precise experiments on human shielding and hull technologies than would have otherwise been possible with other AX weapons.

### 5. Bonus Analysis: Human Shield and Hull AX Resistances

For a long time it was assumed that most, if not all, of the AX damage that impinges a human shield or hull plating is fully mitigated without consequence [3].  Some work had been done in the past that determined the human shield and hull resistance to be 95% and 90% respectively [4].  In this section we definitively address the question of human AX resistances in the modern (i.e. 3.4) era.

The theoretical treatment starts with the first two-component damage equation described in the previous equation.  Given the fact that AX-configured AMCs deal 100% AX damage, we can readily solve the equation for the shield AX damage resistance:

![](https://canonn.science/wp-content/uploads/2019/06/ZZZZ_02_AX_shield_resistance.png)

where *S* is the human target shield strength, *δ* is the full weapon damage figure, *N* is the total number of weapon shots fired, and ∆ is the fraction of the shield strength at a given moment after the Interceptor has activated its shield.  We can adapt the two-component damage equation to the case of hull damage, in which case can solve for the hull AX damage resistance:

![](https://canonn.science/wp-content/uploads/2019/06/ZZZZ_03_AX_hull_resistance.png)

where *H* is the human target hull strength, *A\_R* is the target Armor Rating, *A\_P* is the AMC Armor Piercing, and the other variables are the same as described above.  It should be noted that parameter ∆ and the number of shots fired are values that are measured experimentally, with the former extracted from the left-hand panel of the firing ship.

The human shield resistance to AX damage was determined by performing damage tests against a T-9 with a C7 shield generator fully (i.e. G5) engineered for thermal resistance.  The shield had a strength of 257.8 MJ.  A Krait MkII equipped with four C2 AMCs was used to deal damage to the shield.  Two trials were conducted, and each was broken down into 400-shot segments, and at each point the shield resistance estimate was extracted.  The table below shows the results for both trials.  The result obtained was very consistent at 95.020% AX resistance.

![](https://canonn.science/wp-content/uploads/2019/06/ZZZZ_04_AX_shield_resistance_results.png)

The same type of experiment was conducted versus the hull of a T-9, which consisted of the standard light weight hull, with a total integrity of 864.  It should be noted that the Armor Rating of the T-9 is 65.  The AMC damage per shot is 2.2, and the corresponding Armor Piercing is 37.  The table below shows the results for two trials at various points in the data acquisition process.  Given the relatively high integrity of the standard T-9 hull, the results had some degree of error to start with, but as more shots were fired the AX resistance measurement got progressively more precise.  The final measurement of the hull resistance to AX damage is 90.034%. Both trials yielded the same exact results.

![](https://canonn.science/wp-content/uploads/2019/06/ZZZZ_05_AX_hull_resistance_results.png)

We should note that the final figure of around 90% was confirmed by estimating the hull damage with two additional methods: 1) looking at the repair time of a C5 repair limpet, and 2) estimating the amount of hull lost by simply looking at the cost required to repair the hull at the station.  In all cases the final estimate was still 90% AX resistance.

### 6. Summary and Outlook

A two-component damage model was used to estimate the damage partitioning of the newly developed AMCs.  It was found that, when configured with AX ammunition, the AMCs deal 100% AX damage.  That fact was leveraged to get a handle on the AX resistance of human technology. It was found that human shields have an AX resistance of 95% and human armor plating has a resistance of 90%.  By corollary, other facts about about the AMC were confirmed, such as damage per shot and Armor Piercing.

### 7. Acknowledgements

This study was funded in part by the Canonn Interstellar Research Group and the Xeno Investigation division of the Anti-Xeno Initiative.

We would like to thank CMDR Joulupunikki for participating in this study. In addition to piloting the target vessel, he provided the engineered shields for this analysis as well as peripheral hardware. We would also like to thank CMDR 100.RUB for providing guidance, words of wisdom, and becoming a strong advocate for transparency in weapon documentation for the benefit of the galactic community.

### 8. References

[1] Galnet, “Zende Partners Claim Victory”, https://community.elitedangerous.com/galnet/uid/5cefe7ab9b38db6a762655b6

[2] CMDR Maligno, “Thargoid Interceptor Shield Analysis”, https://canonn.science/codex/thargoid-interceptor-shield-analysis/

[3] CMDR 100.Rub, “The Information Problem”, https://forums.frontier.co.uk/threads/the-information-problem.448887/

[4] CMDR Taleden, Pilot’s Federation Forum Topic, https://forums.frontier.co.uk/threads/elite-shipyard.92900/page-50#post-7824049