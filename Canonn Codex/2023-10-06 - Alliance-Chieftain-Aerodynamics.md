## Alliance Chieftain Aerodynamics

Published: 06 Oct 2023 on Canonn (https://canonn.science/codex/research-notes/alliance-chieftain-aerodynamics/)

Content: The Alliance Chieftain is a medium size ship manufactured by Lakon Spaceways. It was designed to be sturdy yet maneuverable compared to other ships in its size and weight class making it a common choice for anti-Thargoid combat. At first look it appears at least semi-aerodynamic due to the presence of what appears to be wings, but as shown below this is not exactly the case. The following reference quantities were used when performing the analysis for the Alliance Chieftain. Additionally, diagrams of the Alliance Chieftain geometry and CG used in the analysis are provided. All gifs shown below can be found here:https://imgur.com/a/VntmLxC.

| S\_ref (Reference Area) | 558.9221m^2 |
| --- | --- |
| b\_ref (Reference Span) | 58.5623m |
| c\_ref (Reference Chord) | 67.9611m |

Reference Values

| CG\_x | 31.5556m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 6.9490m from bottom-most surface |

CG Approximation Values

![](https://canonn.science/wp-content/uploads/2023/10/image-25-1024x399.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2023/10/image-26-1024x676.png)Isometric View

![](https://canonn.science/wp-content/uploads/2023/10/image-27-1024x687.png)Vehicle Diagram

## Lift and Drag

Despite having what appears to be wings the Alliance Chieftain boasts an incredibly low lift to drag ratio. This begs the question if it should be classified as a lifting body or a winged vehicle as it really does neither well, suffering at both low and high speeds. The odd shape of the vehicle’s body leads to a cambered like shape that shifts the zero-lift point to about 2 degrees angle of attack. Despite having what appears to be wings, the poor lifting characteristics of the Alliance Chieftain require a reevaluation of these structures. Upon closer inspection, they are really thick flat plates that lack any sort of aerodynamic shaping. As such, these should be considered structure struts, not wings, as they hinder flight more then they support it. The fuselage of the Alliance Chieftain is fairly aerodynamic but it’s engine nacelles create excessive drag since they are effectively flat surfaces perpendicular to the flow. Air-breathing engines also have large frontal areas projected perpendicular to the flow to capture the incoming air for use in combustion. Unfortunately, the frontal faces on the Alliance Chieftain can not be considered flow-through since they are the exhaust vents for the reverse thrusters. These large flat faces increase the drag on the entire vehicle to the point where it’s no better then a sphere or angled cube with the same frontal area. Due to the shaping of the ship, the lowest drag occurs at a small angle of attack, roughly 2-to-4 degrees. Finally, the Alliance Chieftain experiences relatively standard Mach-drag divergence with the highest drag occurring around Mach 1.25 and tapering off from there.

![](https://canonn.science/wp-content/uploads/2023/10/image-28-1024x615.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_MachSweep.gif)

## Pitch Stability

At first glance, the Alliance Chieftain appears to be incredibly fickle, flipping between stable and unstable as it transitions through the various Mach regimes. This could indicate poor flying qualities that would make it a dangerous ship to fly. Upon closer inspection however it is noticed that while the previous statement is technically true, a quick glance at the static margin indicates that the ship could be considered neutrally stable. This type of stability is desired for maneuverable aircraft; as an example, most 20^th^ century fighter jets were neutrally stable. Being too stable results in the craft being unable to maneuver rapidly while being too unstable results in a craft that is impossible to control, but by keeping a craft neutrally stable the best of both worlds can be achieved (with proper flight control systems). It is also observed that it keeps this neutral stability across a range of angles of attack which is again, desirable. While the previous discussion praises the Alliance Chieftain, it is still not without its faults with regards to pitch stability. Note that with the exception of one point at the transonic Mach number, the pitching moment never crosses the horizontal axis. As such, the vehicle is not capable of aerodynamic trim and thrusters would be required to constantly be active to keep it trimmed. Fortunately, due to its neutral stability, not much thrust would be required, but it is still an unnecessary expense.

![](https://canonn.science/wp-content/uploads/2023/10/image-29-1024x615.png)Pitch Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Transonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Hypersonic_AlphaSweep.gif)

## Yaw Stability

At a glace it might be assumed the Alliance Chieftain would perform better in yaw due to having what appears to be vertical stabilizers. On aircraft the vertical stabilizers aids in both yaw and roll stability, as well as providing yaw control if a rudder is present. However, the vertical stabilizers on the Alliance Chieftain are horribly undersized and shadowed by the body, providing almost no additional yaw stability. In fact, generally speaking, the vehicle is unstable in yaw except at the supersonic Mach number (that said it becomes unstable again in the hypersonic regime so this segment of stability is short lived). The yaw plane static margin once again shows that the ship is basically neutrally stable in yaw as well. This, paired with the pitch stability observations, makes sense for a ship that markets itself on its maneuverability.

![](https://canonn.science/wp-content/uploads/2023/10/image-30-1024x617.png)Yaw Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Transonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Hypersonic_BetaSweep.gif)

## Roll Stability

The Alliance Chieftain showed very interesting roll characteristics that could potentially make it a challenge to fly without proper training, flipping back and forth between roll stable and unstable. However, it is really another case of being neutrally stable in roll with the aerodynamics really providing no advantage or disadvantage.

![](https://canonn.science/wp-content/uploads/2023/10/image-31.png)Roll Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Transonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Hypersonic_PhiSweep.gif)

## Conclusion

It has been semi-expected that the Alliance Chieftain would be at least reasonably aerodynamic but as shown other than retaining neutral stability across a range of flight conditions, it is aerodynamically a very poor vehicle. This could lead to dangerous situations where its aerodynamic shape gives the false impression of being a good ship for thick atmospheric flight, leading to overconfidence in pilots. Additionally, a potentially dangerous flaw was uncovered when analyzing the hypersonic solution. Due to the blunt features on the vehicle, bow shocks form on both the engine nacelles and the nose. These shocks appear to coalesce right in front of the wing (note that the shock shapes will change as a function of Mach number) and could impinge on the shock coming off the thick wing/strut leading to create shock-on-shock interactions. Shock-on-shock interactions are highly studied phenomena, the results of which depend on the angle at which one shock impinges on another. Of these interactions, none is more deadly than the Edney Type IV interaction which sends a supersonic jet through the shock and straight onto the surface. An observation that is made between supersonic and hypersonic aircraft is how blunt the surfaces are on the hypersonic vehicle. For example, think of the 20^th^ century Apollo capsule compared to fighter jets of the same era. This is because hypersonic flow is characterized by extremely high temperatures and while blunt objects create more drag, they also generate a bow shock. These bow shocks, compared to an attached oblique shock, push the highest temperature regions of the flow away from the body allowing the surface to remain relatively cooler. When an Edney Type IV interaction occurs, this high energy fluid is allowed to impinge directly on the surface of the body leading to catastrophic failure of the surface, as shown when a X-15 research aircraft was almost lost when a shock interaction of this type ate through the Inconel, a high temperature metal alloy, strut holding on a test engine in a configuration not too far removed from what is observed on the Alliance Chieftain. This type of deadly shock-on-shock interaction is an inherently unsteady phenomena, requiring significantly more computing time and power then has been allocated for this study. As such, Canonn highly recommends the Pilots Federation perform detailed analysis and/or extensive wind tunnel testing on the Alliance Chieftain as even flying through tenuous atmospheres could pose risky for this vehicle.

![](https://canonn.science/wp-content/uploads/2023/10/image-32-1024x577.png)Shock-on-Shock Interaction

![](https://canonn.science/wp-content/uploads/2023/10/image-33.png)X-15 Shock-on-Shock Interaction

![](https://canonn.science/wp-content/uploads/2023/10/AllianceChieftain_Scalar-Pretty-Picture.png)Alliance Chieftain in Flight