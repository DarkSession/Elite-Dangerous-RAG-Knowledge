## Sidewinder MkI Aerodynamics

Published: 06 Oct 2023 on Canonn (https://canonn.science/codex/research-notes/sidewinder-mki-aerodynamics/)

Content: The Sidewinder MkI is a small size ship manufactured by Faulcon DeLacy. It is the first ship that most newly registers Commanders fly, often as a loaned ship from the Pilots Federation. Its versatility and low price make it a popular entry-level vessel but despite that it is considered one of the most maneuverable ships on the market. The following reference quantities were used when performing the analysis for the Sidewinder MkI. Additionally, diagrams of the Sidewinder MkI geometry and CG used in the analysis are provided. All gifs shown below can be found here: https://imgur.com/a/RrKFFi5.

| S\_ref (Reference Area) | 81.5340m^2 |
| --- | --- |
| b\_ref (Reference Span) | 21.3678m |
| c\_ref (Reference Chord) | 13.6450m |

Reference Values

| CG\_x | 6.7773m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 2.4983m from bottom-most surface |

CG Approximation Values

![](https://canonn.science/wp-content/uploads/2023/10/image-15-1024x269.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2023/10/image-16-1024x471.png)Isometric View

![](https://canonn.science/wp-content/uploads/2023/10/image-17-953x1024.png)Vehicle Diagram

## Lift and Drag

Since the Sidewinder MkI lacks any wings, it can be classified as a lifting body. These types of vehicles have decent lifting capability at high speeds but suffer at lower speeds. This is confirmed by the Sidewinder MkI having a lift-to-drag ratio like the 20^th^ century Space Shuttle at hypersonic speeds but unable to obtain significantly higher ratios at slower speeds. It is also interesting to note that the top to bottom asymmetry of the Sidewinder MkI causes a noticeable shift in the lift curve. Like a cambered airfoil, the lift is not zero at 0 degrees angle of attack. Instead at subsonic and transonic speeds the lift is zero at ~4 degrees angle of attack, shifting to negative angles of attack at higher speeds. This is due to the lower frontal wedge of the ship that was found to cause other interesting aerodynamic phenomena with regards to pitch, discussed below. As expected, due to the large, untampered, flat back surface the Sidewinder MkI has a large drag coefficient, at best akin to a sphere with the same frontal area and at worst an angled cube. Once again, due to the asymmetric nature between the top and bottom halves, the lowest drag occurs at an angle of attack, usually in the 2-to-4-degree range. Finally, the Sidewinder MkI experiences relatively standard Mach-drag divergence with the highest drag occurring around Mach 1.50 and tapering off from there.

![](https://canonn.science/wp-content/uploads/2023/10/image-20-1024x640.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_MachSweep.gif)

## Pitch Stability

Due to a lack of tail and short airframe, the Sidewinder MkI was found to be unstable in pitch across all Mach regimes studied. The stability does improve at higher Mach numbers but at subsonic speeds it is roughly 0.15 calibers unstable indicating the CG would have to shift at least 2 meters forward from the approximated position for the ship to be stable. An interesting phenomenon was observed at supersonic and hypersonic speeds, the Sidewinder MkI only had positive (nose-up) pitching moments across all angles of attack. Since the pitching moment curve never crosses zero, there is no aerodynamic trim point, and the thrusters would be required to constantly be active to push the nose down. Without knowing the power of the thrusters, it cannot be said if this is a major issue, but at the very least it does require the ship to burn additional fuel just to maintain stability.

![](https://canonn.science/wp-content/uploads/2023/10/image-21-1024x615.png)Pitch Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Transonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Hypersonic_AlphaSweep.gif)

## Yaw Stability

While the Sidewinder MkI was found to be unstable in pitch, it was found to be stable in yaw for the most part. The airframe is about 0.1 calibers stable in yaw (the CP is about 2.1 meters aft of the CG). An interesting observation with the yawing moment is how well behaved it is, i.e., does not change drastically across flight regimes, except for transonic flight. For transonic flight, it is unstable in yaw for small angles of sideslip but fortunately becomes stable again at higher angles preventing full yaw divergence. This sudden change in flight characteristics as the ship transitions from subsonic to supersonic flight could potentially be devastating if unexpected by the pilot or proper control laws are not in place to dampen this effect. This was unexpected from a ship marketed to new pilots.

![](https://canonn.science/wp-content/uploads/2023/10/image-22-1024x615.png)Yaw Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Transonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Hypersonic_BetaSweep.gif)

## Roll Stability

The Sidewinder MkI showed very interesting roll characteristics that could potentially make it challenge to fly without proper training. In both subsonic and supersonic flight, the airframe is shown to be roll stable, but in transonic flight the behavior flips to become roll unstable, and at hypersonic flight it is effectively neutrally stable. This constantly flip-flopping behavior is again unexpected from a ship marketed towards new Commanders. The small values however indicate this moment is small and perhaps not a deal killer.

![](https://canonn.science/wp-content/uploads/2023/10/image-23.png)Roll Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Transonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Hypersonic_PhiSweep.gif)

## Conclusion

While it was not expected that the Sidewinder MkI would be a particularly aerodynamic ship, one object of study stood out as the most interesting that required additional review. As stated, it was found that the airframe has an odd pitch divergence where at above supersonic Mach numbers it does not want to pitch down. As shown in the figure below, this is clearly a function of Mach. It was found this behavior was caused by the forward lower wedge on the Sidewinder MkI’s leading edge. Due to the large angle of this wedge with respect to the oncoming flow, a stronger shock is formed on the bottom surface then on the top, highly pressurizing it and creating a Z-axis force that resulted in a positive moment. Had this study included more angles of attack outside the selected range, it is expected that this effect would have tapered off at low enough angles of attack to shield the bottom wedge.

![](https://canonn.science/wp-content/uploads/2023/10/image-24.png)Pitch Divergence

Since the Sidewinder MkI appears to have a lifting body style planform, it was expected it would be a “bank-to-turn” airframe which was confirmed by analyzing the forces. The airframe is almost 10 times more effective in generating Z-axis force than it is Y-axis force. This means that to change direction the airframe should be rolled towards a target and the stick pulled back (or pushed forward, but positive Gs are safer for manned airframes). This type of maneuver style is called bank-to-turn. The alternate flight methodology, “skid-to-turn” would put the airframe into a sideslip to point the nose at the target without rolling but due to the poor sideslip and yaw performance, this type of flight methodology is not recommended for the Sidewinder MkI.

Overall, the Sidewinder MkI is not a very good airframe having high drag for its size and stability characteristics that drastically change across flight regime. That said, with a trained pilot and advanced control laws, the Sidewinder MkI could still safely transverse an atmosphere.

![](https://canonn.science/wp-content/uploads/2023/10/SidewinderMkI_Scalar-Pretty-Picture.png)Sidewinder MkI in Flight