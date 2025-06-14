# Background Simulation
|  | **Parts of this article have been identified as out of date.** Please update this article to reflect the current version of the game, and remove this template when finished.
<br>Many blanks/unknowns, particularly in tables. Limited references provided, possibly non-authoritative.<br> |
| --- | --- |

The **Background Simulation** is dynamic, complex and reflects the evolution of the galaxy with ever changing power and system influence of factions in response to player behaviour. Every Station, Surface Port and Settlement has its own demands and supply that change dynamically.

The BGS does not only change the galaxy for everybody. Everyone can change the BGS as well. Whatever players do inside Settlements has a direct outcome on the factions that control it. The BGS dictates who controls parts of a star system.^[1]^

*ED* players on different platforms cannot directly play with each other. However, players on every platform affect the same shared galaxy, star systems, factions and the dynamic Background Simulation.

## 

Contents

- 1 Overview
- 2 Influence
- 3 Faction States
- 4 State Flow
- 5 State Effects
- 6 Expansion
- 7 Asset Ownership & Conflict States
- 8 Server Updates
- 9 Videos
- 10 External links
- 11 References

## Overview

*Elite Dangerous* features a complex Background Simulation which drives a dynamic system of ever-changing power and influence. Struggles between minor factions are commonplace throughout the galaxy and are influenced by the actions of player Commanders both incidentally and intentionally through the mission system and other activities. Many players enjoy actively supporting a chosen minor faction by helping to win its battles, defend its territory, and expand its operations into nearby star systems. In essence, player actions can turn a minor faction into an interstellar empire that controls dozens of systems. While altering the local politics of a star system can be done by a lone Commander, it is far easier to support a minor faction with a large, coordinated group, especially as the minor faction grows.

Star systems, as in previous *Elite* games, differ in their forms of government, local laws, and economies. However, both regular player activity, such as trading or piracy, and special missions will affect how the ruling faction of the system develops over time. Pirate activity, for instance, will lower the security level in the system and prompt its government to issue missions to counter the pirate threat; in extreme circumstances this might prompt a visit from a Capital Ship. Trading will affect the standard of living and wealth of the population, as well as prices which depend on temporary gluts and shortages.

## Influence

Minor Factions are political entities with star systems that vie against each other to control assets within the star system. Assets of a system include Starports, Outposts, Installations, Surface Ports and Settlements. The strength of a faction’s presence in a system is displayed as their influence level. Influence levels are increased, or reduced by player activity such as completing missions, trading and bounty hunting. Whichever minor faction controls the primary Starport for the system is considered the controlling faction for the system.

The minor faction that owns a port will determine the laws for the jurisdiction for that port. This is commonly dictated by the superpower allegiance of the minor faction, and its government type.

Currently, there is little direct linkage between minor factions and Powers, although Powers can influence certain aspects like laws and markets within their dominion and grant state and influence bonuses to allied minor factions. Conversely, minor factions that are diametrically opposed to a Power make that system more costly to control. This connection between Powers and minor factions is something we’d like to strengthen during season 2 and beyond.

There is a cap on the amount a faction can change in influence per day, which is determined by: the size of population (the bigger the harder), the faction state, the amount of player activity that day, and any power influence on that system. Influence is calculated on an approximately daily tick.

## Faction States

As well as affecting influence, player actions also drive the state of that system which can include a range of effects from famine through to lockdowns, the following actions have different strength effects on economic states:

| ACTIONS | Boom | Bust | Civil Unrest | Famine | Outbreak | Lockdown | INFLUENCE |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Trade | ↑<br> | ↓<br> |  | ↓ (Food)<br> | ↓ (Meds)<br> |  | **↑** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Smuggling | ↑<br> | ↓<br> | ↑ (Weapons)<br> | ↓ (Food)<br> | ↓ (Meds)<br> | ↑ (Weapons)<br> | **↓** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Redeeming Bounties |  |  | ↓<br> |  |  | ↓<br> | **↑** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Redeeming Combat Bonds |  |  | ↓<br> |  |  |  | **↑** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Selling Exploration Data | ↑<br> | ↓<br> |  | ↓<br> | ↓<br> |  | **↑** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Murder |  |  | ↑<br> |  |  | ↑<br> | **↓** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Other Crime |  |  | ↑ |  |  | ↑ | **↓** |
| --- | --- | --- | --- | --- | --- | --- | --- |

## State Flow

Player activities shown in the Actions Table above, and through related missions, push the faction towards and away from economic states by adding points to pools. Once the pool is large enough it will queue the state with a countdown after which the event will trigger, assuming it has the largest pool.

When a state triggers, all other economic state pools are reset to 0 apart from Outbreak and Famine which are halved, unless it is Famine or Outbreak when they are all reduced to 0.

All States have a countdown before they trigger, a minimum and maximum duration, and a cool down before which the state cannot occur again, even if it has been interrupted.

| ACTIONS | Countdown | Min Length | Max Length | Cooldown |
| --- | --- | --- | --- | --- |
| Expansion | 5 | 3 | 5 | 2 |
| --- | --- | --- | --- | --- |
| Investment | ? | ? | ? | ? |
| --- | --- | --- | --- | --- |
| War | 3 | 4 | 28 | 0 |
| --- | --- | --- | --- | --- |
| Civil War | 3 | 4 | 28 | 0 |
| --- | --- | --- | --- | --- |
| Election | 3 | 3 | 5 | 2 |
| --- | --- | --- | --- | --- |
| Boom | 2 | 3 | 28 | 3 |
| --- | --- | --- | --- | --- |
| Bust | 2 | 3 | 28 | 3 |
| --- | --- | --- | --- | --- |
| Civil Unrest | 1 | 3 | 7 | 7 |
| --- | --- | --- | --- | --- |
| Famine | 3 | 3 | 28 | 25 |
| --- | --- | --- | --- | --- |
| Outbreak | 4 | 3 | 28 | 7 |
| --- | --- | --- | --- | --- |
| Lockdown | 1 | 3 | 14 | 1 |
| --- | --- | --- | --- | --- |
| Retreat | 1 | 5 | 5 | 3 |
| --- | --- | --- | --- | --- |

## State Effects

When certain states are active, they can modify which player activities can affect the faction’s influence:

| STATE | EFFECT |
| --- | --- |
| Expansion | All activities contribute. |
| --- | --- |
| Investment | Triggered by a failed expansion and significantly increases development level for a short time and actions contribute to a longer range expansion next attempt. |
| --- | --- |
| War | Influence is frozen. Completing more combat missions and actions than the opposing faction for four cumulative days over a seven-day period will result in a large increase in influence at the end of the war and a large decrease in influence for the opposing faction. Can only apply to non-native factions or to native factions in conflict with a non-native faction. |
| --- | --- |
| Civil War | Influence is frozen. Completing more combat missions and actions than the opposing faction for four cumulative days over a seven-day period will result in a large increase in influence at the end of the war and a large decrease in influence for the opposing faction. Can only apply to native factions. |
| --- | --- |
| Election | Influence is frozen. Completing more non-combat missions and actions than the opposing faction for four cumulative days over a seven-day period will result in a large increase in influence at the end of the election and a large decrease in influence for the opposing faction. Can only apply to non-anarchy factions of the same government category (social, autocratic, or corporate) as the opposing faction. |
| --- | --- |
| Boom | Trade contributions double in this state. |
| --- | --- |
| Bust | Trade double reduction of boom but no influence. |
| --- | --- |
| Civil Unrest | Collecting bounties has double the effect and system security lowers. |
| --- | --- |
| Famine | Combat actions and missions do not contribute but food has double the effect. |
| --- | --- |
| Outbreak | Combat actions and missions do not contribute but Medicine has double the effect. |
| --- | --- |
| Lockdown | Activities have no effect for the duration and many station services are shut down. |
| --- | --- |
| Retreat | Triggered when a faction falls below 2.5% and owns no assets in any system other than their home. If the situation is not changed quickly they will leave the system. |
| --- | --- |

States also modify the “wealth”, “security”, “development level” and “standard of living” stats if the faction controls a star system. The prices and production of certain market goods are also affected when economic and conflict states are active.

## Expansion

A faction will attempt to expand to a new system when their influence reaches 75% in a system and they are not being blocked by a conflict state. At the end of the expansion state the faction attempts to expand to the nearest system that is:  

- within 20 ly
- fewer than 7 factions present

If successful, the faction loses 15% of their influence in the system they expanded from. During the expansion state, they gain bonus influence for actions in that new system. If there is no valid system within 20 ly, the expansion will fail and the faction will go into an investment state where actions will allow the next expansion to reach 10 ly further. If a system is full but there is a faction with very low influence presence the expansion will work and immediately trigger an invasion war in the new system.

During the expansion state, the faction will offer expansions missions and ask for exploration data to be sold at the system they are expanding from. These actions have an unquantified positive effect on the starting influence in their new system.

## Asset Ownership & Conflict States

Assets are ground ports/bases and space stations/outposts. These assets allow the owner faction to be affected by player actions as described above. One asset in every system is the controlling asset whose owner controls the system, setting the local laws and bounties. 

The ownership of an asset can change at the conclusion of one of the following states: 

- War (if a faction is invading from another star system)
- Civil War
- Election

To trigger a conflict state the two factions must either be at roughly equal influence or a non-controlling faction must get over 60% influence in the system influence to trigger a conflict with the system controller. No conflicts can happen below 7% influence.

These conflict states take priority over economic states and will block or end them early. Conflicts cannot end before their minimum duration. Conflicts that reach their maximum duration are considered to end in a ceasefire, and no assets change owners. A faction can only take part in a single conflict, no matter how many systems they are present in.

The state of a War or an Election is decided on a daily basis, with the faction completing the most relevant missions (and/or winning the most Conflict Zone battles in the case of a War or Civil War) winning the day. The conflict state concludes after seven days, at which point the winning faction (the faction which won the most days) gains a significant increase to influence, the losing faction gains a significant decrease to influence, and the most valuable asset owned by the losing faction is transferred to the winning faction. This is always the asset which controls the system if the system controller loses the conflict.

What conflict state occurs depends on the type of factions involved. The minor factions are grouped in three categories by goverment type. The factions in a category do not wage Wars against the factions in the same category. Instead, they hold Elections. The categories are: 

- social - Communist, Confederacy, Cooperative, Democracy, Theocracy
- autocratic - Dictatorship, Feudal, Patronage, Prison Colony
- corporate - Corporate

The Anarchistic factions are excluded from this and always move in system's faction leaderboard through War.

It is also possible to skip a conflict state and have a "coup". This only occurs if a faction rises with excessively increased influence to dominate the system and the rival faction controlling the system drops to very low influence and has no positive player activity. This rare event leads to the changing of the controlling asset instantly but it may be delayed by some states.^[verification overdue]^

## Server Updates

Every week the servers that host the Milky Way go offline at ~7am UTC for a scheduled service to allow the Galaxy's persistent data to update:^[2]^

- Star System & Station / Outpost ruling minor factions, alignment, and available commodities & services
- Powerplay Control / Exploited Systems
- Addition of new Community Goals

This update usually takes between 30 and 60 minutes, during which time you cannot login to the Milky Way.