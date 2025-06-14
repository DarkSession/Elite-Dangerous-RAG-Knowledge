## Beluga Liner Aerodynamics

Published: 23 Apr 2025 on Canonn (https://canonn.science/codex/research-notes/beluga-liner-aerodynamics/)

Content: The Beluga Liner is a large ship manufactured by Saud Kruger. It was designed as a high-end passenger ship, able to accommodate luxury-tier cabins and carry a vast number of passengers. In recent years it has also seen service as a hospital/evacuation ship, pulling larges quantities of survivors from burning stations that had been attacked by Thargoids. Many believe the Beluga Liner, like other sleek ships from Saud Kruger, to be aerodynamically friendly, a claim which will be evaluated here. The following reference quantities were used when performing the analysis for the Beluga Liner. Additionally, diagrams of the Beluga Liner geometry and CG used in the analysis are provided. All gifs shown below can be found here: https://imgur.com/a/aVkAngC

| S\_ref (Reference Area) | 1861.0820 m^2 |
| --- | --- |
| b\_ref (Reference Span) | 131.5101 m |
| c\_ref (Reference Chord) | 208.9861 m |

Reference Values

| CG\_x | 105.1942 m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 19.7373 m from bottom-most surface |

![](https://canonn.science/wp-content/uploads/2025/04/image-7-1024x912.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2025/04/image-8-1024x672.png)Isometric View

![](https://canonn.science/wp-content/uploads/2025/04/image-10-1024x480.png)Vehicle Diagram

## Lift and Drag

The sleek nature of the Beluga with relatively large aerodynamic surfaces would lead many to believe it is an aerodynamic vessel. The good news is this is true, at least compared to other analyzed ships. The Beluga Liner does not have the lowest drag of the analyzed large ships but it does have the highest lift-to-drag ratio of them by almost a factor of 2x, at subsonic speeds. This indicates the Beluga Liner is aerodynamically efficient. Like other ships that have large angled foreheads, the Beluga Liner’s drag bucket is shifted slightly towards the positive angles of attack, but this is a minor effect thanks to the gradual slope and somewhat countered by the lower angled “chin”. The large forward aerodynamic surfaces are not fully enveloped by the shock of the nose, leading to higher drag. If the Beluga Liner did not have these forward surfaces it might be the lowest drag large ship.

![](https://canonn.science/wp-content/uploads/2025/04/image-12-1024x614.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://i.imgur.com/QjBamF8.gif)Beluga Liner Mach Sweep

## Pitch Stability

The large aerodynamics surfaces on the back of the Beluga Liner indicate a likely stable platform, which is true at subsonic and supersonic speeds where the Beluga Liner has a neutrally stable leaning towards stable airframe. This would be expected from a dedicated passenger ship where stability beat maneuverability from a safety and comfort perspective.  Unfortunately, due to the onset of severe shock shading at transonic speeds the Beluga Liner’s stability suddenly flips at positive angles of attack becoming noticeably unstable. This could lead to ships accelerating from launch or decelerating after reentry to have a sudden change in behavior from otherwise very nice flying characteristics. If the forward control surfaces were smaller, or non-existent, the ship would be more stable about the theorized center of gravity. 

![](https://canonn.science/wp-content/uploads/2025/04/image-13-1024x614.png)Pitch Stability Characteristics

![](https://i.imgur.com/taMUliL.gif)

![](https://i.imgur.com/DzZsMMq.gif)

![](https://i.imgur.com/9DuPMV2.gif)

![](https://i.imgur.com/GDySWsw.gif)

## Yaw Stability

Unlike many of the analyzed ships so far, the Beluga Liner has surfaces that could be considered vertical stabilizers. This leads to Beluga Liner to be decently stable in yaw especially at larger angles of sideslip. While there are some small subsonic oddities near zero beta, also seen supersonically due to multiple shock interactions between the surfaces, this should be correctable and would not lead to much divergence. This is a good choice for a dedicated passenger liner but care should be table to ensure those small near-zero beta instabilities don’t result in the ship swaying side to side which made induce “sea sickness” in the passengers. 

![](https://canonn.science/wp-content/uploads/2025/04/image-15-1024x614.png)Yaw Stability Characteristics

![](https://i.imgur.com/z0j74m7.gif)

![](https://i.imgur.com/2qNCJma.gif)

![](https://i.imgur.com/l6niz87.gif)

![](https://i.imgur.com/JvwJFeI.gif)

## Roll Stability

In another plus for the Beluga Liner, it is also stable in roll. It has an odd combination of dihedral and anhedral surfaces but the net effect is a rolling moment of similar magnitude to the yawing moment with inherent stability. Across all Mach regimes, the Beluga Liner wants to fly flat, a great characteristic for a passenger carrier.

![](https://canonn.science/wp-content/uploads/2025/04/image-17.png)Roll Stability Characteristics

![](https://i.imgur.com/OHXce2z.gif)

![](https://i.imgur.com/MQOl4Sh.gif)

![](https://i.imgur.com/KtFb63i.gif)

![](https://i.imgur.com/Ic7Jzi5.gif)

## Conclusion

The Beluga Liner, unlike most craft reviewed thus far, is an aerodynamically friendly ship. It boasts the highest lift-to-drag ratio of any ship seen thus far and is mostly stable in all three channels. Care should be taken since this stability could be called into question if the estimated CG location is wrong and located further aft than estimated. All that said, all things equal, it has nice aerodynamic qualities for a spacecraft. It should be noted that these characteristics would also hold true in water, where the ship would in all likelihood be subsonic. While not used in this capacity yet it has been conceptualized the Saud Kruger liners would have this capability. The only difference between air and water in this analysis would be the incompressible nature (which is captured with the subsonic analysis) and higher density (captured by using coefficients instead of dimensional values). The largest improvement that could be made to the Belgua Liner would be the removal of the forward surfaces. This would pull the center of pressure aft, increasing the stability. Additionally, since these surfaces are anhedral, their removal would further increase the roll stability. 

![](https://canonn.science/wp-content/uploads/2025/04/BelugaLiner_v2_Scalar-Pretty-Picture-1.png)Beluga Liner in Flight